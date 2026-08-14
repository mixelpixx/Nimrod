<p align="center">
  <img src="https://nimrod.orchis.ai/assets/icon.svg" width="96" alt="Nimrod">
</p>

<h1 align="center">Nimrod</h1>

<p align="center"><b>Web research your agent can actually use.</b><br>
Quality-scored Google search, clean webpage extraction, and deep multi-source
research for Claude — over the Model Context Protocol.</p>

<p align="center">
  <a href="https://nimrod.orchis.ai">Website</a> ·
  <a href="https://nimrod.orchis.ai/docs.html">Docs</a> ·
  <a href="https://nimrod.orchis.ai/#pricing">Pricing</a> ·
  <a href="https://nimrod.orchis.ai/portal">Portal</a>
</p>

---

## What it is

Nimrod gives Claude four research tools:

| Tool | What it does | Cost |
|---|---|---|
| `google_search` | Organic Google results with quality scores, authority ratings, and source-type classification | 1 credit |
| `extract_webpage_content` | Any URL → clean markdown, boilerplate stripped | free |
| `extract_multiple_webpages` | Up to 5 URLs, fetched concurrently | free |
| `research_topic` | Search → rank → dedupe → extract → synthesis, in one call | 1 credit per search |

Why not just let the model search? Because raw search is where agent runs go to
die: Nimrod returns **ranked evidence instead of SEO sludge**, as
**token-efficient markdown instead of raw HTML**, with deterministic costs
(1 credit = 1 search) and date/site/language control.

New accounts start with a **free 50-credit trial** — no card required.

## Get connected

**Claude.ai & Claude Desktop (zero install):** Settings → Connectors → Add
custom connector → paste `https://nimrod.orchis.ai/mcp` → sign in with your
email. Done.

**Claude Code (hosted):**

```bash
claude mcp add nimrod --transport http https://nimrod.orchis.ai/mcp \
  --header "Authorization: Bearer nmk_your_key"
```

**Nimrod Desktop (full toolkit — recommended for power users):** a locally
installed MCP server with six research skills, a deep-research agent, and
local extraction that never touches your credits. Grab it from
[**Releases**](../../releases):

- **Windows** — `nimrod.mcpb` for Claude Desktop (double-click, paste key),
  or `nimrod-desktop.exe` for Claude Code: `nimrod-desktop setup`, then
  `claude mcp add nimrod -- path\to\nimrod-desktop.exe`
- **macOS** — `nimrod-desktop-macos` (universal: Apple Silicon + Intel):
  `chmod +x` it, then a one-time
  `xattr -d com.apple.quarantine nimrod-desktop-macos` (not yet
  Apple-signed), then `setup` and `claude mcp add` as above
- **Linux** — `nimrod-desktop-linux`: `chmod +x`, `setup`, `claude mcp add`

## Built to pair

Run Nimrod beside your other MCP tools — like
[Konnect](https://github.com/mixelpixx/Konnect) for KiCAD: live parts data from your EDA
workflow, live web research from Nimrod, one agent, no stale training cutoff.

## Support

Docs: [nimrod.orchis.ai/docs.html](https://nimrod.orchis.ai/docs.html) ·
Email: [admin@orchis.ai](mailto:admin@orchis.ai) ·
[Terms](https://nimrod.orchis.ai/terms.html) ·
[Privacy](https://nimrod.orchis.ai/privacy.html)

---

<sub>The original open-source BYOK server this project grew from is preserved
on the <code>historical-oss</code> branch (unmaintained).</sub>
