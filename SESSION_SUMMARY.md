# Daggerheart Hexcrawl - Session Summary

## Resume

```
cd ~/daggerheart-hexcrawl && cat SESSION_SUMMARY.md
```

Then tell Claude:
```
Continue working on the daggerheart-hexcrawl project. Read the session
summary above. The GitHub commit credential needs fixing first (see
BLOCKING section), then we can test the full pipeline end-to-end and
add Discord posting.
```

---

## BLOCKING: GitHub Credential Fix Needed

The "Commit to GitHub" node in the Hex Generator workflow gets a **403** with fine-grained PATs. The fix:

1. Create a **classic PAT** (NOT fine-grained) at GitHub > Settings > Developer settings > Personal access tokens > Tokens (classic)
2. Check the **`repo`** scope
3. Update the `"n8n Daggerheart hexcrawl"` credential in n8n with the new `ghp_` token
4. Test by triggering the webhook: `curl -s -X POST "https://n8n.elmertucker.space/webhook/generate-hex" -H "Content-Type: application/json" -d '{"prompt": "test hex", "tier": 2}'`

The `gh` CLI OAuth token works fine for writes — only the n8n fine-grained PATs fail.

---

## What We've Built

### GitHub Infrastructure (Complete)
- **Repo:** https://github.com/ElmerTucker/daggerheart-hexcrawl
- **Live Site:** https://elmertucker.github.io/daggerheart-hexcrawl/
- Jekyll-based GitHub Pages site with Daggerheart-themed styling
- Hex layout template rendering all schema fields correctly
- Sample hex: The Scorched Hollow (demonstrates full schema)

### Schema (Complete)
Corrected to match actual Daggerheart rules:
- Environment stat blocks with: name, tier, type, description, impulses, difficulty, potential_adversaries, features
- Features have: name, type (Passive/Action/Reaction), fear_cost, description, questions
- Hex includes: environment, encounters (Fear/Hope), factions, points_of_interest, npcs, adventure_sites, tags

### n8n Workflows

**Live in n8n instance at https://n8n.elmertucker.space:**

| Workflow | ID | Status | Purpose |
|----------|-----|--------|---------|
| Daggerheart Hex Generator | `reaYbkLnmtJqYIW6JO9tk` | Active | Main workflow - generates hex, converts to Jekyll, commits to GitHub |
| Daggerheart Environment Generator | `zUy_6zJJwpX6NXCL89wgD` | Active | Sub-workflow called as AI tool for environment stat blocks |

**Hex Generator Architecture (13 nodes):**
- Manual Trigger + Webhook Trigger (`POST /webhook/generate-hex`) + Schedule Trigger
- Set Defaults picks random region/terrain/tier if not provided
- GitHub node fetches existing hexes to calculate next hex ID
- AI Agent (GPT-4.1) generates hex JSON, calling Environment Generator tool
- Validate & Parse JSON ensures schema compliance
- **Convert to Jekyll Markdown** (Code node) - serializes hex JSON to YAML frontmatter
- **Commit to GitHub** (GitHub node) - creates `_hexes/{id}-{slug}.md` in repo
- Output Hex JSON (NoOp passthrough)

**Environment Generator Architecture (4 nodes):**
- Trigger receives name/tier/type/theme from parent workflow
- Build Prompt constructs system+user messages (handles both structured params AND query-string input from AI agent)
- **Call OpenAI** (HTTP Request to Chat Completions API) - replaced broken n8n OpenAI Responses API node
- Validate Environment ensures structured features with name/type/fear_cost/description/questions

**Credentials in use:**
- `80PBLan4eZN2zkcz` / "GitHub account" - used by Get Existing Hexes (read-only, works)
- `W6v9CvDIyjEs4pD5` / "n8n Daggerheart hexcrawl" - used by Commit to GitHub (NEEDS classic PAT)
- `8GhcxLxmH9v4rL19` / "OpenAi account" - used by AI agent and Environment Generator HTTP Request

**Old/Duplicate workflows to clean up:**
- `R9kNMeZ9V4Fh4e7rAuRQu` - "Hex Generation" (old version)
- `g8-rp7pX7X0jO5JNtFhOT` - "Daggerheart Environment Generator" (old version)

### Bugs Fixed This Session
1. **Merge Triggers disabled** - removed node, connected triggers directly to Set Defaults
2. **Environment Generator input parsing** - AI agent sends `{query: "name: X\ntier: 2\n..."}` but sub-workflow expected structured fields. Fixed Build Prompt to parse query strings.
3. **OpenAI Responses API broken** - n8n's `@n8n/n8n-nodes-langchain.openAi` node returned generic "Hello!" response, ignoring system prompt. Replaced with HTTP Request node calling Chat Completions API directly.
4. **Validation output format** - Updated to handle Chat Completions response format (`choices[0].message.content`)
5. **Features as strings** - Environment Generator now returns properly structured feature objects (verified in execution 128)

## Issue Tracker Status

| Issue | Title | Status |
|-------|-------|--------|
| #1 | Create hex crawl GitHub repo + GitHub Pages site | ✅ Closed |
| #2 | Design n8n agentic workflow for hex generation | ✅ Complete |
| #3 | Build n8n GitHub + Discord posting pipeline | 🔄 In Progress (GitHub commit built, needs credential fix + Discord) |
| #4 | Add search and vector DB integration | ⏳ Future |
| #5 | Refine hex schema based on Daggerheart source | ✅ Done |

## Campaign Context (Beast Feast)

- Monster Hunter meets Delicious in Dungeon
- Setting: Plover Caves / Southern Depths
- Regions: The Jasmine Reaches, The Bitter Depths, The Forgotten Vaults, The Descent Shafts, The Titan's Tomb, Halfway Station, The Great Descent, The Weeping Gallery, The Bone Gardens

## Next Steps

### Immediate: Fix GitHub Credential
See BLOCKING section above. Once the classic PAT is in place, re-test end-to-end.

### Then: Issue #3 Remaining Work

1. **Fix hex ID calculation** - Currently returning "001" even when hex files exist. May need to also update "Get Existing Hexes" to use the new credential, or check that the `_hexes` path is correct.

2. **Post to Discord**
   - Format hex as Discord embed with title, region, environment summary, encounter names
   - Link to GitHub Pages URL
   - Send via Discord webhook

3. **Optional: Fine-tune scheduling**
   - Schedule Trigger already added in UI
   - Configure cron for desired frequency

### Future Enhancements (Issue #4)
- Vector DB integration for semantic search across hexes
- RAG for generating hexes that connect to existing content
- Search UI on GitHub Pages site

## Key Files

```
/home/elmer/daggerheart-hexcrawl/
├── _config.yml                 # Jekyll config
├── _layouts/
│   ├── default.html
│   └── hex.html                # Hex page template
├── _hexes/
│   ├── 001-the-scorched-hollow.md          # Sample hex
│   └── 001-smoldering-archive-vaults.md    # Generated by workflow (bad features)
├── assets/css/style.css        # Daggerheart theme CSS
├── index.html                  # Hex index page
├── README.md                   # Schema documentation
├── n8n/
│   ├── hex-generator-workflow.json         # Reference (live version in n8n)
│   └── environment-generator-workflow.json # Reference (live version in n8n)
└── SESSION_SUMMARY.md          # This file
```

## API Access

n8n API key is in `~/.claude/settings.json` under mcpServers.n8n.env.

```bash
# List workflows
curl -s -X GET "https://n8n.elmertucker.space/api/v1/workflows" \
  -H "X-N8N-API-KEY: $N8N_API_KEY" | jq '.data[] | {id, name, active}'

# Trigger hex generation
curl -s -X POST "https://n8n.elmertucker.space/webhook/generate-hex" \
  -H "Content-Type: application/json" \
  -d '{"prompt": "description of hex", "tier": 2}'

# Check latest execution
curl -s -X GET "https://n8n.elmertucker.space/api/v1/executions?workflowId=reaYbkLnmtJqYIW6JO9tk&limit=1" \
  -H "X-N8N-API-KEY: $N8N_API_KEY" | jq '.data[0] | {id, status}'
```
