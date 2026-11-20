# Step 5. GitHub for dummies (back up your code)

⏱️ 10 minutes · 💰 $0 (free GitHub account)

**Goal:** a safe copy of your site in the cloud, with every change saved, so you can always undo.

GitHub sounds like a developer thing. You won't need to memorise a single command; Claude does the typing.

## What they do (Claude: walk them through it, one step at a time)

1. Create a free account at https://github.com
2. Click **New repository**. Name it something simple like `my-business-website`. Choose **Private**. Don't add a README (this project already has one). Click **Create repository**.
3. Copy the repository address it shows (it ends in `.git`) and paste it to Claude.

## What Claude does

1. Check the project is committed (`git status`). Commit anything outstanding.
2. Check nothing private is about to be pushed: no `.env` files, keys or passwords anywhere in the project. `workspace/` is fine to push to a **private** repo; it's their business notes.
3. Point the project at their repo: `git remote set-url origin <their address>` (or `git remote add origin <their address>` if there's no origin yet). This kit was cloned from Jef's public repo, so `origin` starts out pointing there. It must point at **their** repo before pushing.
4. Push: `git push -u origin main`.
5. The first push opens a GitHub sign-in in their browser. **They sign in themselves.** Never ask for their GitHub password or a token in the chat.
6. Confirm by asking them to refresh the GitHub page and see their files.

## Why it matters

Every change you push is saved with a date. If you ever hate an update, you can go back to yesterday's version in seconds. Just ask Claude: "Undo the last change to the home page."

**Done when:** their files show in their own private GitHub repository.
