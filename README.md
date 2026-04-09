# argmax.codes — deployment notes

Pure static site. No build step. No JS. No backend.

## Structure

```
argmax/
├── index.md                    # root directory (human + agent readable)
├── agents.json                 # serve at /.well-known/agents.json
├── robots.txt
├── sitemap.md
├── clients/
│   ├── text2list.md
│   ├── lounge.md
│   ├── theagentdeck.md
│   ├── compyoot.md
│   ├── icp.md
│   ├── kktrophy.md
│   ├── johnphotography.md
│   └── rinasbasement.md
├── lounge/
│   └── index.md
└── agents/
    └── index.md
```

## Deploy options

**Cloudflare Pages** (easiest, free):
1. Push to a GitHub repo.
2. Connect to Pages, build command empty, output dir `/`.
3. Point `argmax.codes` DNS at Pages.
4. Add a `_headers` file if you want `Content-Type: text/markdown; charset=utf-8` on `.md` so browsers render them as text.

**GitHub Pages:** same idea, uses Jekyll by default — add an empty `.nojekyll` file to skip it and serve raw.

**Railway / Vercel / Netlify:** all work, overkill for this.

## Important: serve .md as text/markdown

Agents parsing this will expect raw markdown. On Cloudflare Pages, add
`_headers`:

```
/*.md
  Content-Type: text/markdown; charset=utf-8

/agents.json
  Content-Type: application/json
```

## The /.well-known/ convention

Move `agents.json` to `/.well-known/agents.json` at deploy time. That's
the emerging convention for agent-discoverable metadata (same folder as
`security.txt`, `openid-configuration`, etc).

## Adding a new property

1. Create `clients/newthing.md` with frontmatter.
2. Add an entry to `agents.json`.
3. Add the path to `sitemap.md`.
4. Link it from `index.md`.

That's it. No database, no CMS, no admin panel. Clawd can do this with a
single handoff.
