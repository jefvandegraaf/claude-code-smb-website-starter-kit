# Step 1. Do some damn research

⏱️ 1.5 to 2+ hours · 💰 $0 manual, or included with Claude Pro

**Goal:** know who you're up against locally, and collect design inspiration from businesses like yours in *other* cities.

Skipping this is the number one reason AI-built sites come out generic. The businesses that matter are the ones:

- ranking first in Google Search
- showing in the top 3 spots of Google Maps
- being mentioned in AI Overviews and AI answers

**Outputs:**
- `workspace/research/competitors.md`: 5 to 10 local competitors with URL, price tier, main selling point, what they do well, and gaps
- `workspace/research/inspiration.md`: 4 to 8 out-of-market sites you like, with *why* (layout, mood, booking flow, pricing clarity)

---

## For Claude: how to run this step

1. Using the city and business type from intake, run the AI research prompts below yourself (web search) and draft `competitors.md`.
2. Ask the owner to do the Google searches below on **their own phone or browser**, because Google results depend on location. Ask them to share screenshots or paste what they see, especially the Maps top 3. Merge that into `competitors.md`.
3. Ask: "Which 2 or 3 of these do you lose customers to most often?" Mark those as primary rivals.
4. Run the inspiration prompts and draft `inspiration.md`. Ask them to open the links and tell you which ones *feel* right. Keep only the ones they like.
5. Summarise the 3 biggest gaps you see (things competitors all fail at) and save them at the top of `competitors.md`. They feed Step 2.

**Done when:** both files exist, the owner has confirmed the primary rivals, and they've picked at least 2 inspiration sites.

---

## Google searches (do these on your own device)

| Angle | Search | What it shows |
|---|---|---|
| Core proximity | `[business type] near me` | The Map Pack top 3 for people near you |
| Service-specific | `[specific service] near me` (e.g. `emergency water heater repair near me`) | Businesses that steal one profitable service from you |
| Neighbourhood | `[business type] in [neighbourhood or postcode]` | Who dominates pockets of your city |
| Map view | `map:[City] [business type]` | A geographic cluster of physical competitors |
| No directories | `[business type] [City] -site:yelp.com -site:thumbtack.com -site:angi.com -site:yellowpages.com` | Real independent business sites only |
| Service-page spy | `inurl:[service-slug] "[City]"` (e.g. `inurl:bridal-makeup "Austin"`) | Competitors with dedicated pages per service |
| Roundups | `intitle:"best [business type]" "[City]"` | Local press and "best of" lists |
| Lookalikes | `related:[competitorwebsite.com]` | Sites with a similar audience |

## AI research prompts

**1. Direct local rivals**
> Search the web and list the top 10 direct competitors for a [business type] in [City/Neighbourhood] that offer [primary service]. Include their website URL, price tier, and main selling point.

**2. Service-specific overlap**
> I run a [business type] in [City]. Identify businesses that may not share my exact business model, but directly compete with me for [specific service]. List their websites and how they package this service.

**3. Problem-based (indirect)**
> My target audience in [City] is trying to solve [core customer problem]. Aside from [your business type], what other local businesses, services, or alternatives are capturing their budget for this need?

**4. Search and ad competitors**
> Act as an SEO strategist. If a customer in [City] searches for [service + city] or [problem keyword], which local businesses dominate the organic results, the Google Map Pack, and paid ads?

**5. Adjacent / upstream rivals**
> List local businesses in [City] that serve [target customer, e.g. new homeowners] and have recently expanded into offering [your service] as an add-on or bundle.

**6. Weakness and gap finder**
> Analyse the websites and public customer reviews of [Competitor 1], [Competitor 2], and [Competitor 3] in [City]. What recurring complaints do customers have, and what sub-services or customer segments are all three failing to serve?

---

## Design inspiration (out-of-market only)

Look at businesses like yours in **other cities and countries**, so you can borrow ideas without copying a neighbour.

| Angle | Search |
|---|---|
| Design-hub cities | `"[business type]" ("Melbourne" OR "Copenhagen" OR "Austin" OR "London") -site:yelp.com` |
| Modern platforms | `"[business type]" ("powered by webflow" OR "made with squarespace")` |
| Pricing pages | `inurl:pricing "[business type]"` or `inurl:packages "[business type]"` |
| Other countries | `site:.co.uk "[business type]" "[service]"` (or `.com.au`, `.ca`, `.se`) |
| Showcases | `site:awwwards.com "[industry]"` or `site:siteinspire.com "[industry]"` |

**AI inspiration prompts**

> Find 8 independent [business type] in design-forward cities like [Melbourne, Copenhagen, Austin, London, Tokyo]. Focus on modern branding, strong photography and clean web design. Share their URLs and describe their visual style.

> Search for top-rated [business type] websites in the US, UK and Australia that offer [service, e.g. monthly plans or custom packages]. Give me 6 sites that explain pricing clearly and make booking effortless.

> I want my [business type] website to feel [3 adjectives, e.g. warm, editorial, minimalist]. Find 6 non-competing businesses in [other countries/cities], in my industry or adjacent lifestyle spaces, that nail this. Break down what makes their homepage work.

> Identify 5 [business type] businesses in [New York, Toronto, Sydney] with a frictionless mobile experience and standout booking or quote-request flows. Explain what they do well.

> What are the most innovative [business type] brands doing with their websites in [Scandinavia, Japan, Western Europe]? Give me 5 real examples with links and note UI or copy trends I could adapt.
