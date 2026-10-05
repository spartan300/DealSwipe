# DealSwipe

Swipe through Slickdeals front-page deals and it learns what you like. It's a single static `index.html`, with no backend and no build step.

- **→ Want**, **← Nope**, **↑ Too pricey** (watches for a ~20% lower price on similar items), **↓ Have it** (hides similar deals). **Space** skips, **Z** undoes, **Enter** opens the deal.
- All preferences live only in your browser's localStorage. Use Export/Import in ⚙︎ to move them between devices.
- Refreshes every 5 minutes. A hot match or a price drop triggers a notification while a tab is open.
- The feed is fetched through free public CORS proxies (allorigins → codetabs → corsproxy.io). Under ⚙︎ you can set your own proxy.

## Host on GitHub Pages
1. Push this folder to a GitHub repo.
2. Settings → Pages → Deploy from branch → `main` / root.
3. Open `https://<you>.github.io/<repo>/`.

Running it locally: `python3 -m http.server`, then open http://localhost:8000.
