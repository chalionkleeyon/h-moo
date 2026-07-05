# Our Honeymoon 💍

A little web app for our honeymoon: an interactive map, an itinerary, and a
dedicated page for each leg of the trip. Everything is editable right in the
browser — no coding needed.

## What's in here

- `index.html` — the whole app (map, pages, editor). One file, no build step.
- `data.json` — the trip content (starts with 3 sample legs). This is what you edit.
- `README.md` — this file.

The map uses free OpenStreetMap tiles via Leaflet, so there are **no API keys
and no accounts** to set up. It will run for free on GitHub Pages forever.

---

## Put it online with GitHub Pages (about 5 minutes)

1. Go to https://github.com and sign in (create a free account if needed).
2. Click **New repository**. Name it something like `honeymoon`. Set it to
   **Public**. Click **Create repository**.
3. On the new repo page, click **uploading an existing file**.
4. Drag in `index.html`, `data.json`, and `README.md`. Click **Commit changes**.
5. Go to **Settings → Pages** (left sidebar).
6. Under **Build and deployment → Source**, choose **Deploy from a branch**.
   Pick branch **main** and folder **/ (root)**. Click **Save**.
7. Wait ~1 minute, refresh, and GitHub shows your live link, like
   `https://YOURNAME.github.io/honeymoon/`. Share it with your partner. 🎉

> Want it private? GitHub Pages needs a Public repo on the free plan. The link
> is unguessable but technically public. That's fine for most people; if you
> want it truly private, tell me and I'll suggest an alternative host.

---

## How to edit the trip

**The easy way — right in the app:**

1. Open your live site (or open `index.html` on your computer).
2. Click **Edit** in the top-right.
3. On the home screen you can set the trip title/dates, manage your **activity
   colors** (Transportation, Dining, Boat outing, Winery, etc. — rename, recolor,
   or add your own), and add/reorder/delete legs.
4. Click **"Edit this leg & its days"** on any leg to edit everything about it,
   including a **day-by-day itinerary**. Add a day, pick its date (the weekday
   fills in automatically), then add activities with a time, description, a
   color-coded type, and optional notes. Reorder or delete days and activities freely.
5. To set a leg's map location, type latitude/longitude **or just click the map**
   to drop the pin — the coordinates fill in automatically.
6. Click **Done editing** to preview.

Your changes save automatically **in your browser** as you type.

**To make edits permanent and shared with your partner:**

1. Click **Export** (top-right). This downloads an updated `data.json`.
2. In your GitHub repo, click `data.json` → the pencil ✏️ → delete the contents,
   paste the new file (or use **Upload files** to replace it) → **Commit changes**.
3. Within a minute the live site updates for both of you.

**Photos:** paste any image URL into the Photo field. Easiest option: upload the
image to your repo too, then use a relative URL like `photos/paris.jpg`.

---

## Good to know

- **Import** lets you load a `data.json` file back in (handy for restoring or
  moving between devices).
- The footer link **"reset to saved file"** clears your browser edits and reloads
  whatever is committed in `data.json`.
- Opening `index.html` directly (double-click) works too, but browsers block
  reading `data.json` from a local file, so it falls back to the built-in sample.
  For local editing, use the live GitHub Pages link, or run a tiny local server:
  `python3 -m http.server` then visit `http://localhost:8000`.
