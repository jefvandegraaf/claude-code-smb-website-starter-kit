# Step 3. Design tokens, then your core pages

⏱️ 1 to 2 hours · 💰 included with Claude Pro

**Goal:** a site that looks custom without copying anyone, built from your real words.

## A word on copying

AI can read any website's code and clone it. Scammers and lazy agencies do exactly that, and some get caught and called out publicly. Don't be that business. Instead of "make me a knockoff of this", you'll pull out the **design tokens** (colour mood, typography, spacing, corner style) from your Step 1 inspiration sites and blend them with your own brand.

**Outputs:**
- `workspace/design-tokens.md`
- `site/assets/css/styles.css` (tokens as CSS variables at the top)
- the 5 core pages in `site/`

---

## For Claude: how to run this step

### 3.1 Design tokens
1. Ask for **screenshots** of 2 or 3 inspiration sites they picked in Step 1 (or open them yourself if you have a browser tool), and any existing logo or brand colours they already use. Existing brand colours win over inspiration.
2. Run the four token prompts below. For fonts, show 3 pairings and let them choose.
3. Check every text/background colour pair meets WCAG AA contrast (4.5:1 for body text, 3:1 for large text). Fix any that fail and say so.
4. Save `workspace/design-tokens.md`, then write the CSS variables block into `site/assets/css/styles.css`.

### 3.2 Core pages
1. Build pages in this order: Home, Contact, Services, 2 to 3 service pages, About. (Contact early, because every other page links to it.)
2. Follow every rule under "Build rules" in `CLAUDE.md`. The Home page replaces the placeholder `site/index.html` completely, including its `noindex` tag. Restyle `site/404.html` with the shared header and footer too, and keep its `noindex`.
3. After **each page**: preview it (Step 4 explains how), check it at 375px and desktop, list any `[NEEDS: …]` markers, and get their OK before the next page.
4. Commit after each approved page.

**Done when:** all core pages are approved, every page shares one header and footer, and the only remaining `[NEEDS: …]` markers are ones they've agreed to fill before launch.

---

## Token prompts (use with screenshots)

**1. Colour palette and contrast**
> I'm uploading screenshots of 2–3 websites whose vibe I love (from other industries or cities). Extract an original colour palette inspired by their mood, not an exact copy, for my [business type]. Give hex codes for: Background, Surface/Card, Primary text, Muted text, Primary brand colour, and a high-contrast CTA accent. Make sure everything meets WCAG AA.

**2. Typography pairing**
> Based on these screenshots and my brand personality ([3 adjectives]), recommend 3 free Google Font pairings (one heading font, one body font). Specify weights, line heights and letter-spacing for H1, H2, H3 and body copy.

**3. UI style and component rules**
> Analyse the UI style of these sites and write short design rules for my website: corner radius for buttons and cards, shadow depth, section padding and card style. Clean, modern, mobile-first.

**4. Save as `design-tokens.md`**
> Combine the colours, font rules and UI rules into `design-tokens.md`, plus a ready-to-use CSS variables block.

---

## The 5 core pages

| Page | Must include |
|---|---|
| **Home** | Hero with a clear value proposition and one main button · trust bar (reviews, credentials) · services overview cards · "Why us" using the real USP · pricing preview · FAQ · final call to action |
| **Services** | All core services · "How working with us works" in 3 steps · pricing philosophy with ballpark ranges · links to each service page |
| **Service pages (2–3)** | Service-specific hero · the exact frustrations this service fixes · what's included · pricing range · top 4 objections answered · short quote/booking form |
| **About** | Origin story (why you care) · what you do differently from typical competitors in your city · real founder/team photo slots · call to action |
| **Contact / Quote** | Short form (name, contact, service, brief details) · clickable phone, email, hours, service area · "What happens after you hit send" |

**Example prompt (Home)**
> Using `brand-context.md` for copy and `design-tokens.md` for styling, build the Home page for my [business type]. Sections: 1) hero with a punchy headline, subheadline and main button, 2) social proof bar, 3) service overview cards, 4) "Why choose us" using our real USP, 5) a transparent pricing preview, 6) an objection-handling FAQ. Layout note: [e.g. generous whitespace and bold section headers like inspiration site A].

**Example prompt (Service page)**
> Build a dedicated, SEO-focused page for [specific service] in [City], using `brand-context.md` and `design-tokens.md`. Focus on the customer frustrations for this one service, list what's included, show realistic pricing, answer the top 4 objections, and end with a fast quote form.

---

## Later: expansion pages that bring in free leads

Once the core site is live, these are quick to add with Claude Code:

- **Area pages:** "[Service] in [Suburb]" for each area you serve (only with something genuinely local to say on each, never copy-paste pages with the town name swapped)
- **Case studies / before-and-after:** a real customer's problem, the fix, the result
- **"Who we serve" pages:** homeowners vs property managers vs commercial
- **Cost guides:** "How much does [service] cost in [City]?"
- **Comparison pages:** "Us vs big national chains", "DIY vs hiring a pro"
- **Process pages:** your method, warranty or guarantee in detail
- **Industry pages:** one per industry you serve, in their language
- **Estimate calculator:** an instant ballpark quote in exchange for an email or phone number
