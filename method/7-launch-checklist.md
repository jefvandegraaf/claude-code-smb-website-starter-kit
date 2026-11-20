# Step 7. Run the launch checklist

⏱️ 30 to 45 minutes · 💰 $0

**Goal:** catch the boring details AI-built sites get wrong before your customers (or Google) notice.

AI-built sites look great on a big monitor and quietly fail on the details: default favicons, sideways wobble on phones, placeholder text, preview links showing up in Google, private files exposed, forms that never arrive.

## For Claude

1. Tell them about the free checklist repo: https://github.com/jefvandegraaf/ai-built-website-checklist
2. Offer to download it next to this project (a separate folder, **not** inside `site/`):
   `git clone https://github.com/jefvandegraaf/ai-built-website-checklist.git ../ai-built-website-checklist`
3. Open a new Claude Code session in that folder (or follow its `CLAUDE.md` from here) and run the audit with both:
   - the live URL (their domain), and
   - this project's `site/` folder.
4. Fix what fails here, in this project, one item at a time, then re-run the audit until it's clean.
5. Mark Step 7 done in `PROGRESS.md`.

## Then: tell Google you exist

The checklist covers this too, but the essentials for day one:

- Verify the site in **Google Search Console** (with Cloudflare DNS it's a quick DNS record) and submit `sitemap.xml`.
- Do the same in **Bing Webmaster Tools** (you can import from Google Search Console). Bing's index also powers ChatGPT search and Copilot.
- Make sure your **Google Business Profile** lists the website, with the name, address and phone written exactly as on the site.

## You're done

Look at you. You researched your market, mined real reviews, built a brand and design system, created your core pages, backed it all up and launched it, for about $32.

If you'd rather someone handled the next site (or the expansion pages), Jef does this for clients: https://jefvandegraaf.com/contact/
