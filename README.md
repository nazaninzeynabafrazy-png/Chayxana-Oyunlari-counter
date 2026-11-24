# Çayxana Oyunları counter

The online service for The Parlour: live player count, invite counter, clans (names, avatars, preset chat, weekly ranking, shared chest) and optional G-rated GIFs.

- `cloudflare-worker.js` — the service (Cloudflare Worker with one Durable Object).
- `wrangler.toml` — its settings. Deploy with `npx wrangler deploy` (Workers & Pages, no build command).
- Optional secret `GIPHY_KEY` turns on GIFs in chat.

Check it works: open `/count` (shows `{"users":0}`) and `/clan/list` (shows `{"ok":true,"clans":[]}`).
