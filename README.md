# daily-ai-deep-dive-feed

Public RSS proxy feed for **The Daily AI Deep Dive** podcast — one celebrated
AI research paper per day, explained properly (agentic AI, physical AI,
biomedical AI, frontier research, and more).

The show's audio and episode metadata are produced daily on the muse.ai
podcast feed, whose RSS template does not include the `<itunes:author>` and
`<itunes:owner>` tags that Apple Podcasts Connect, Spotify for Creators, and
YouTube's RSS ingestion require. This repo hosts a byte-faithful proxy copy
of that feed with those tags added.

- **Submit this URL to directories:** `https://srjain04.github.io/daily-ai-deep-dive-feed/feed.xml`
- `sync/build_feed.py` rebuilds `feed.xml` from the source feed.
- `.github/workflows/sync-feed.yml` runs it every morning after the new
  episode publishes, and commits the result when it changes.
