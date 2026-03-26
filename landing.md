Publish and read on the open web. Own both sides of the feed.

RSS Lobster is a personal publishing and reading system built on RSS. Publish from your phone to your own site. Subscribe to feeds and read them in the same CLI. No algorithms. No platform.

**Cost:** $12/year for a domain. Hosting: free.

## Get started

```bash
npm install -g rsslobster
rsslobster onboard
```

Three questions. Thirty seconds. Your site is live.

## Publish

Send a message from Telegram. The lobster classifies it, generates static HTML with inlined CSS, updates your RSS feed, and deploys via git push. Under 4 seconds. Your words are never rewritten.

| Type | You send | What you get |
|------|----------|--------------|
| **Microblog** | A short thought | Tweet-style post |
| **Post** | Longer writing | Full article with title |
| **Image** | Photo with caption | Image post with `<figure>` |
| **Link** | URL with commentary | Link card with metadata |

## Read

```bash
rsslobster feeds add https://simonwillison.net
rsslobster feeds
```

Subscribe. Poll. Star what matters. Share back to your site as link posts. Read something interesting, run `feeds share 3`, and it's published on your site. One tool, both directions.

## How it works

**Publish side:** phone → classify → HTML + RSS → git push → deploy → live in 4 seconds

**Read side:** subscribe → poll → notify → star → share → publish as link post on your site

The two sides compose. You read something, share it, your subscribers get it in their readers. The open web feedback loop.

Files as the API. Git is the database. Zero JavaScript in output.

## Setup is progressive

```bash
rsslobster enable telegram   # publish from your phone
rsslobster enable model      # AI-powered classification
rsslobster enable deploy     # auto-deploy via git push
```

Each capability is independent. Use what you need, skip what you don't.

## Open source

MIT licensed. [GitHub](https://github.com/HectorZarate/rsslobster) · [npm](https://www.npmjs.com/package/rsslobster)
