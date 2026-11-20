# Step 6. Launch on Cloudflare (for free)

⏱️ 15 minutes · 💰 $0 hosting + about $12/year for a domain

**Goal:** your site on the real internet, with free hosting, free SSL and a preview link for every change.

## Part A: get a live `.pages.dev` link

Claude: walk them through it one step at a time. Cloudflare's dashboard changes often, so if a label doesn't match, ask them what they see.

1. Create a free account at https://cloudflare.com
2. In the left sidebar open **Workers & Pages** → **Create** → the **Pages** tab → **Connect to Git**.
3. Connect GitHub and select the `my-business-website` repository.
4. Build settings (this part matters):
   - **Framework preset:** None
   - **Build command:** leave empty
   - **Build output directory:** `site`
5. Click **Save and Deploy**.

A minute or two later they get a link like `my-business-website.pages.dev` that anyone can open.

> Why `site`? Only that folder goes public. Your notes, research, this kit's instructions and `CLAUDE.md` stay private. If the output directory is left blank, Cloudflare publishes the whole project, and anyone could read your brand notes at `/workspace/brand-context.md`.

**Claude, verify it:** open `https://<their-project>.pages.dev/CLAUDE.md`. It must **not** load (404 is correct). If it loads, the output directory is wrong. Fix it before going further.

## Part B: preview links for every change

Every time you push a change to GitHub, Cloudflare builds it and gives that version its own preview link. Open it **on your phone** before you call anything finished.

`.pages.dev` links are full public copies of your site. The `site/_headers` file in this kit already tells Google not to index them (`X-Robots-Tag: noindex`), so they won't compete with your real domain. Leave that file in place.

## Part C: connect your real domain

1. In the Cloudflare project, open **Custom domains** → **Set up a custom domain** → type `yourbusiness.com`.
2. Follow the prompts. If the domain is with Cloudflare already, it's one click. If it's elsewhere, Cloudflare tells you which DNS records to change.
3. Add the `www.` version too, and have it redirect to the main one (or the other way round). Pick one and stick to it.
4. SSL (the padlock) is set up automatically.

**Tip:** if you haven't bought a domain yet, Cloudflare Registrar sells domains at wholesale cost with no markup and no sneaky renewal price hikes.

## Claude: before you call it launched

1. Every canonical tag, `og:url`, `sitemap.xml` entry and the `Sitemap:` line in `robots.txt` use the real domain. Search `site/` for `pages.dev`, `localhost` and `[NEEDS: domain]`. There should be none.
2. Check the live domain is **not** sending `noindex` (only `.pages.dev` should).
3. If they had an old website, list its old URLs and add 301 redirects to the matching new pages in `site/_redirects` (format: `/old-page/ /new-page/ 301`). Losing old URLs loses their Google rankings overnight.
4. Commit and push.

**Done when:** the site loads on their domain with the padlock, and `CLAUDE.md` doesn't load on either the domain or `.pages.dev`.
