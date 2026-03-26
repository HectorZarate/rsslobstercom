Publish and read on the open web. Own both sides of the feed.

RSS Lobster is a personal publishing and reading system built on RSS. You publish from your phone to your own site. You subscribe to feeds and read them in the same place. No algorithms. No platform. Just the protocol the web already agreed on.

**Cost:** $12/year for a domain. Hosting: free.

## Get started

```bash
npm install -g rsslobster
rsslobster onboard
```

Three questions. Thirty seconds. Your site is live.

## Publish from your phone

Send a message from Telegram. The lobster classifies it, generates a static HTML page with inlined CSS, updates your RSS and JSON feeds, commits to git, and deploys. Under 4 seconds end-to-end.

Your words are never rewritten — the LLM classifies metadata only.

| Type | You send | Output |
|------|----------|--------|
| **Micro** | A short thought | Tweet-style post |
| **Post** | Longer writing | Full article with title |
| **Image** | Photo with caption | Image post |
| **Link** | URL with commentary | Link card with metadata |

## Read the open web

```bash
rsslobster feeds add https://simonwillison.net
rsslobster feeds
```

Subscribe to feeds. Poll them. Star what matters. Share back to your site as link posts. The same CLI that publishes your voice to the open web also reads everyone else's.

Read something interesting → `rsslobster feeds share 3` → it's published on your site. One tool, both directions.

## Progressive setup

Each capability is independent. Use what you need:

```bash
rsslobster enable telegram   # publish from your phone
rsslobster enable model      # AI-powered classification
rsslobster enable deploy     # auto-deploy via git push
```

## Zero JavaScript output

Every generated page uses system fonts, inlined CSS, zero external requests. WCAG AA contrast. Works without JavaScript entirely.

Four style presets: **minimal**, **brutalist**, **magazine**, **terminal**. Every CSS custom property is overridable.

## How it works

```
publish:                              read:

  phone → classify → html + rss         subscribe → poll → notify
            ↓                                        ↓
        git push → deploy               star → share → publish
            ↓                                        ↓
    live in < 4 seconds                 your site ← link post
```

Files as the API. Git is the database. The filesystem is the state.

## Open source

MIT licensed. Built by [Hector Zarate](https://computationalsubstrate.com).

[GitHub](https://github.com/HectorZarate/rsslobster) · [npm](https://www.npmjs.com/package/rsslobster)
