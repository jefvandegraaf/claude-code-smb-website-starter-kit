# Claude Code Small Business Website Starter Kit

> **Beta.** This kit is new and hasn't been run end to end by other business owners yet. It's based on the method I use to build my clients' websites. If a step confuses you or Claude goes off track, please [open an issue](https://github.com/jefvandegraaf/claude-code-smb-website-starter-kit/issues).

**Free to use.** If it helps you, [support the project on my Patron page](https://jefvandegraaf.com/patron/).

Build your own small business website with Claude Code in a weekend, for about **$32**: $20 for a month of Claude Pro and around $12 for a domain. Hosting is free.

This kit turns the 7-step method from **[How to Build a Small Business Website with Claude in 7 Steps](https://jefvandegraaf.com/build-small-business-website-with-claude/)** into a guided build. Open it in Claude Code, and Claude interviews you, researches your competitors, writes from your real words, builds the pages and walks you through launching.

> Out of the box, AI builds generic websites. "Build me a website for my plumbing business in Toronto" gets you fluff that won't rank and won't convince anyone to call. This kit makes Claude do the research and the interview **before** it writes a line of code.

---

## Who it's for

Small business owners (trades, clinics, salons, studios, shops, local services) who want a fast, custom website they own, without a monthly website-builder bill. You don't need to know how to code.

## What you need

- **Claude Pro** (or higher) with **Claude Code**: the desktop app's Code tab, or the terminal version
- A free **GitHub** account (Step 5)
- A free **Cloudflare** account (Step 6)
- A domain name, about $12/year (Cloudflare sells them at cost)
- **4 to 6 hours**, ideally spread over a weekend

## Quickstart

1. **Download this kit.** On GitHub, click **Code → Download ZIP** and unzip it, or run:
   ```
   git clone https://github.com/jefvandegraaf/claude-code-smb-website-starter-kit.git my-business-website
   ```
2. **Open the folder in Claude Code.** In the desktop app, start a new session in the `my-business-website` folder (or run `claude` inside it in a terminal).
3. **Say:** `Let's build my website.`

Claude reads the instructions in `CLAUDE.md` automatically and takes it from there, one question at a time. Close the app whenever you like; type `/next-step` to pick up where you left off, or `/where-am-i` for a quick status.

## The 7 steps

| # | Step | Time |
|---|---|---|
| 1 | Research your local competitors, and find design inspiration from other cities | 1.5–2 hrs |
| 2 | Pull out your real selling points, customer language, pricing and FAQs | 1–1.5 hrs |
| 3 | Turn inspiration into your own design tokens, then build your 5 core pages | 1–2 hrs |
| 4 | Preview the site on your own computer | 15 min |
| 5 | Back it up to GitHub | 10 min |
| 6 | Launch it free on Cloudflare Pages and connect your domain | 15 min |
| 7 | Run the launch checklist | 30–45 min |

Each step has its own guide in [`method/`](method/). You can read them without Claude, and the prompts work in any AI chat too.

## What's in the box

```
CLAUDE.md          Instructions Claude follows (the method, the rules, the guardrails)
PROGRESS.md        Your checklist. Claude ticks it off as you go
method/            One guide per step, with every copy-paste prompt
workspace/         Your private research, brand-context.md and design-tokens.md
site/              Your actual website. The ONLY folder that gets published
examples/          A filled-in example for a (fictional) Toronto plumber
```

**Why `site/` is separate:** when you launch, Cloudflare publishes only the `site/` folder. Your notes, research and these instructions stay private. (If you publish the whole project instead, anyone can read your files at yourdomain.com/CLAUDE.md. It happens a lot.)

## Built-in guardrails

Claude is told to:

- **never invent** reviews, ratings, awards, prices or team members, and to mark gaps as `[NEEDS: …]` instead
- **never clone** a competitor's or inspiration site's layout, copy or images
- check every page on a **375px phone screen**: no sideways wobble, tap-friendly buttons, inputs that don't zoom on iPhone
- keep it **plain HTML and CSS** (fast, nothing to break, nothing to update)
- add the SEO basics: titles, descriptions, canonical tags, sitemap, LocalBusiness schema
- keep `.pages.dev` preview links **out of Google**
- never ask for your passwords or secret keys

## After launch

Run the free **[AI-Built Website Checklist](https://github.com/jefvandegraaf/ai-built-website-checklist)**. It tests your live site and your files for the things AI-built sites get wrong: default favicons, mobile wobble, placeholder text, exposed files, preview links in Google, missing schema, broken forms.

## Found this helpful?

This is free, and it stays free. If it saved you time, money or a developer's invoice, please [leave a tip or become a patron](https://jefvandegraaf.com/patron/): one-off tips start at $3, and monthly support starts at $5. It keeps these tools maintained and updated.

Don't let Jef starve.

[**Support Jef on the Patron page →**](https://jefvandegraaf.com/patron/)

## Rather have it done for you?

I'm Jef van de Graaf. I research, write, design and build small business websites for clients. If you don't have the time (or the interest), [get in touch](https://jefvandegraaf.com/contact/).

## License

- Method, prompts, templates and docs: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Use and adapt them freely, including commercially, as long as you credit **Jef van de Graaf** with a link to https://jefvandegraaf.com/build-small-business-website-with-claude/
- Code and config files: [MIT](LICENSE)
- The website you build with this kit is 100% yours. No credit needed on your site.

See [LICENSE](LICENSE) for details.
