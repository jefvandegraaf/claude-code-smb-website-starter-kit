# Step 2. Pull the gold out of your head (brand context)

⏱️ 1 to 1.5 hours · 💰 included with Claude Pro

**Goal:** capture your real positioning, your customers' real words, honest pricing and the doubts that stop people from calling, all in one file Claude builds from.

If you skip this, AI fills the blanks with soulless corporate fluff. Nobody talks like that, and nobody buys from a website that reads like a toaster manual.

**Output:** `workspace/brand-context.md` (the template is already in that file; fill it in).

---

## For Claude: how to run this step

Work through the five exercises in order. **One question at a time.** Keep their exact words wherever you can.

1. **Review mining.** Ask them to paste 30+ reviews from their top competitors (Google Maps, Yelp, Facebook), both 5-star and 1 to 3-star. Their own reviews too, if they have them. If they can't, offer to find public reviews yourself and say which sources you used. Then run prompt 1.
2. **USP interview.** Run prompt 2 as a real interview: 5 questions, one at a time.
3. **Objections and FAQs.** Run prompt 3, then ask them which objections they actually hear, and how they answer them in real life. Their real answer beats yours.
4. **Pricing.** Ask for their typical range and what moves the price. If they don't want to publish prices, explain the trade-off once ("how much does X cost" searches are some of the most likely to turn into customers) and respect their choice.
5. **Assemble.** Fill in `workspace/brand-context.md`. Read the hero line and the 3 value propositions back to them and get a yes.

**Done when:** every section of `brand-context.md` is filled in or has a `[NEEDS: …]` marker, and they've approved the hero line and value propositions.

---

## The five exercises

**1. Competitor review mining (voice of customer)**
> I'm pasting 30+ customer reviews (5-star and 1–3 star) from my top local competitors in [City]. Give me: 1) the top 5 exact phrases customers use about what they love, 2) the top 5 recurring frustrations or dealbreakers, and 3) suggested website headlines that address those frustrations. Reviews: [paste]

**2. USP and "deal-closer" extraction**
> Interview me to uncover my real unique selling proposition for my [business type]. Ask me 5 sharp questions, one at a time, about why my best customers chose me over competitors, what mistakes other companies make, and the exact phrases I say on sales calls or at the counter that make people say "let's do it". After I answer, summarise my USP into 3 punchy website value propositions.

**3. Objection handling and real FAQs**
> Act as a skeptical first-time customer looking to hire a [business type] for [service]. Based on common industry myths, bad past experiences and hidden worries, list the top 8 objections or questions I'm thinking before I reach out, and help me write honest, reassuring FAQ answers that address each one.

**4. Pricing transparency and anchoring**
> People hate booking a sales call just to get a ballpark price for [service]. My typical range is [e.g. $500–$2,500] depending on [factors]. Write a transparent "How our pricing works" section that gives realistic ranges, explains what drives the price up or down, and positions us as honest and zero-pressure.

**5. Turn it into `brand-context.md`**
> Take everything we just uncovered (USP, review insights, FAQs, pricing, and my brand tone: [e.g. friendly, direct, no-BS]) and format it into `brand-context.md` with sections for Basics, Hero copy, Services, Proof points, Pricing guide, FAQs and Voice.

---

See `examples/toronto-plumber/brand-context.md` for a filled-in example (fictional business).
