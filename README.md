Access the site here -->
https://stemzy.github.io/justview/

this is for viewing multiple streams at once. u can remove or add new streams. WITH LIVE CHAT ACCESS

updates will come soon still thinking of ideas this is just the mockup version of [justview]

---

## Setup: Twitch login (for the followed-channels sidebar)

The sidebar and grid-saving work out of the box. To turn on "Connect Twitch" and see
who you follow, add your Twitch **Client ID**:

1. Go to https://dev.twitch.tv/console/apps and open the **justview** app → **Manage**.
2. Make sure **OAuth Redirect URLs** includes exactly: `https://stemzy.github.io/justview/`
   (add `http://localhost:5500/` too if you test locally).
3. Copy the **Client ID**.
4. Open `index.html`, find the line near the top of the script:
   `var CLIENT_ID = "";`
   and paste your Client ID between the quotes. Save, commit, push.

That's it — the "Connect Twitch" button in the sidebar will now work. The Client ID is
public/safe to commit. There is no Client Secret needed (this is a browser-only login).

## Features
- Add/remove Twitch streams in an auto-arranging grid, with per-stream chat and fullscreen.
- Collapsible sidebar (☰) showing who you follow, live channels first with a LIVE badge and
  viewer counts. Click a channel to add/remove it from the grid.
- Your grid is saved in your browser, so it's still there when you come back.
- Share button copies a link that reopens your exact lineup.
- Installable as an app (PWA) — look for the Install button / browser install icon.
