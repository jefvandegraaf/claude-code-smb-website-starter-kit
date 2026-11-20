# Step 4. Build and preview locally (your private workshop)

⏱️ 15 minutes · 💰 $0

**Goal:** see your site in a browser while you build it.

Everything happens on your own computer first. It's fast and private, and it uses fewer tokens, because Claude edits files directly instead of pasting huge blocks of code into a chat.

## For Claude: how to start the preview

Serve the `site/` folder (not the project root) on port 5830. Try these in order:

1. **Claude desktop app:** use the preview tools with the `site` configuration in `.claude/launch.json`.
2. **Node installed** (`node -v` works): `npx --yes serve site -l 5830`
3. **Python installed** (`python --version` or `python3 --version` works): `python -m http.server 5830 --directory site`
4. **Neither:** explain that the preview needs a small free tool, and offer to walk them through installing Node.js LTS from https://nodejs.org. Don't install anything without their yes.

Then give them the link: **http://localhost:5830**

Run it in the background so you can keep working. Opening `index.html` by double-clicking isn't enough, because links like `/about/` only work through a server.

## Explain this to them once

> **localhost only exists on your computer.** Nobody else can open it. If you text `localhost:5830` to your business partner, it won't load for them. Think of it as your workshop with the blinds drawn. Step 6 gives you a link anyone can open.

## Check on a real phone too

Resizing a desktop browser isn't the same as a phone. After Step 6 you'll have a preview link you can open on your actual phone. That's where you do the final mobile check.

**Done when:** the preview runs and they can click through every page.
