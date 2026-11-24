# Calendar

A hand-drawn weekly planner: month view, a week view with to-do lists, and a scratchpad
you can drag things out of. It installs as an app on your phone ("Add to Home Screen").

**This repo only holds the app's code. No to-dos are stored here.**

- To-dos are saved in the browser on each device.
- Optionally, the app syncs them to a separate **private** GitHub repo that you choose,
  using a fine-grained access token that you paste into the app. The token stays on your
  device and is never part of this code.

## Setting up sync

1. Create a **private** repo (for example `calendar-data`).
2. Create a [fine-grained token](https://github.com/settings/personal-access-tokens/new):
   - Repository access: **Only select repositories** → the private data repo
   - Permissions → Repository → **Contents: Read and write**
3. In the app, tap the sync status under the arrows, then enter your username, the repo
   name and the token. Do this once on each device.

## Running it locally

```sh
python3 -m http.server 8000
# open http://localhost:8000
```
