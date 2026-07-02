[README.md](https://github.com/user-attachments/files/29591428/README.md)
# Orizon Board

A simple, private, Monday.com-style board for tracking yearly goals, monthly/weekly/daily tasks, and client work — built as a single static page, free to host on Netlify.

## Deploy to Netlify (2 minutes, no account setup beyond signing in)

1. Go to https://app.netlify.com and log in (or create a free account).
2. Click **"Add new site" → "Deploy manually"**.
3. Drag the whole `orizon-board` folder (the one containing `index.html`) into the upload box.
4. Netlify gives you a live URL immediately (something like `random-name-123.netlify.app`). You can rename it under **Site settings → Change site name**.

That's it — no build step, no server, nothing to configure.

To update the site later: make changes to `index.html`, then drag the folder in again on the same site's **Deploys** tab (or set up continuous deploy from a GitHub repo if you'd rather not drag files each time).

## How it works

- Everything is stored **in your browser** (localStorage) — nothing is sent to a server, so there's no backend, database, or login involved.
- Because it's stored in the browser, your data lives on **whichever device/browser you use it on**. Use **Export backup** (in the sidebar) regularly, especially before clearing browser data or switching computers, and **Import backup** to restore it. This is also your way to move data between devices.
- Boards, groups (sections), statuses, and colors are all fully editable — add, rename, or delete any of them.

## Using it

- **Boards** (left sidebar): You start with Yearly Goals, Monthly Tasks, Weekly Tasks, and Daily Tasks — but these are just a starting point. Add a board per client, per project, or however you think about your work. Hover a board to rename or delete it.
- **Groups**: Inside a board, group items however makes sense ("This week", "E&V", "Q3"). Add/rename/delete freely.
- **Items** (rows): Title, Status (click the colored pill to change it), Due date & time, Progress %, Client/Tag, and Notes — all editable inline, just click and type.
- **Manage statuses**: Click "⚙ Manage statuses" at the top of a board to rename statuses, change their colors, add new ones (e.g. "Waiting on client"), or remove ones you don't use. Each board has its own set.
- **Today strip**: The bar under the search field automatically surfaces anything due today, overdue, or coming up in the next 7 days, across all boards — so "E&V meeting at 12 today" will show up there without you doing anything extra.
- **Search & filter**: Use the search box to find anything by title, client, or notes. Click a status chip to filter the current board down to just that status.
- **Notifications**: Click "🔔 Enable notifications" once and allow browser permission. While the Orizon Board tab is open, you'll get a desktop notification ~15 minutes before something is due (and again shortly after, if it's still open). Important: this only works while the tab is open in your browser — a static site with no server can't wake your laptop or send notifications while it's closed. If you want reminders even when the tab is closed, the honest options are keeping the tab pinned open, or using a real calendar app (Google/Outlook) for hard deadlines alongside this board for planning.
- **Backup**: "Export backup" downloads a JSON file of everything. "Import backup" restores from one. Worth doing this every so often, or before trying anything risky.

## Notes on scope

This was built to match what you described: a stripped-down, single-user Monday.com alternative — boards, statuses, due dates, progress, client tags, and notifications — without accounts, permissions, automations, or the pricing/complexity that comes with them. If you outgrow it (e.g. need multiple people editing at once), that would need a real backend and is a bigger step up.
