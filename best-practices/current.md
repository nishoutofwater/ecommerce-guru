# Current E-commerce Best Practices

**Last updated:** 2026-11-02
**Update cadence:** weekly (automated research, reviewed by Nish before merge)

Rules for this file:
- Every entry has a date and a source link.
- Summaries are in our own words. No copied paragraphs.
- Vendor or agency sources are marked `[vendor]`; confirm against the primary source (platform docs, regulator, court) before acting on high-stakes items.
- Entries older than 6 months move to `archive.md` unless still current.

---

## 1. Search and discovery

### Google core updates, 2026
- **2026-11-02:** Google ran a spam update and a core update in March 2026, a Discover-only core update in February, and a second broad core update starting 21 May 2026, shortly after Google I/O. The December 2025 core update was reported to raise E-E-A-T expectations for e-commerce review content. Google's stated guidance remains: no specific fixes, build content for people.
  - Sources: [TripleDart update tracker](https://www.tripledart.com/google-algorithm-update-tracker) `[vendor]`, [Search Engine Land, May 2026 core update](https://searchengineland.com/google-may-2026-core-update-rolling-out-now-478430)
  - **Action:** Product and category pages need original, experience-based content (own photos, real testing, specs, FAQs). Thin manufacturer copy is at risk. Review content should show first-hand use.

### Agentic commerce (AI shopping agents)
- **2026-11-02:** Two open protocols now let AI agents browse and buy from stores: ACP (OpenAI and Stripe, Sept 2025, powers ChatGPT Instant Checkout) and UCP (Shopify and Google, Jan 2026). Payment layers include Stripe Shared Payment Tokens, Google AP2, Visa Trusted Agent Protocol and Mastercard Agent Pay. WooCommerce, BigCommerce, Wix, Squarespace and others are listed as supporting agentic channels. Consumer trust in letting AI place orders is still low, but AI-referred retail traffic is growing fast.
  - Source: [Search Engine Journal, agentic commerce guide](https://www.searchenginejournal.com/selling-to-ai-the-complete-guide-to-agentic-commerce/)
  - **Action:**
    1. Clean product data: descriptive titles (material, colour, type), complete descriptions, real-time price and stock.
    2. Full Product schema with nested Offer (price, currency, availability, seller) and AggregateRating where reviews exist.
    3. Check platform agentic channel settings.
    4. Test category visibility by asking ChatGPT, Perplexity and Google AI Mode for recommendations.
    5. Track AI referral traffic separately (ChatGPT adds `utm_source=chatgpt.com`).
  - **Framework link:** Racecar (new discovery engine forming), TPB (agents read perceived-control data such as shipping and returns), 4Ps (Place).

## 2. Paid social (Meta)
- **2026-11-02:** Meta's ranking now relies on AI systems (Andromeda for retrieval, GEM and a Generative Recommender for ranking). Creative quality and diversity now drive targeting in Advantage+; near-identical creatives are grouped and count as one. A Creative Diversity score rates ad sets. Advantage+ Creative now rewrites text in images and generates variants by default, so review auto-enhancement settings. Threads became a default placement in October 2026 (bids can be reduced, not fully removed). Customer Lifecycle Strategy toggle steers spend to new customers. Meta is testing AI-generated landing pages on a small share of impressions, where pixels and GA4 may not fire. Updated ad terms allowing site crawling for AI training take effect 20 Nov 2026.
  - Source: [Common Thread Collective, Meta ads changes 2026](https://commonthreadco.com/blogs/coachs-corner/meta-ads-changes-2026) `[vendor]`
  - **Action:** Plan creative in distinct concepts (angles, formats, people), not variations of one shot. Audit auto-enhancement defaults for brand and compliance risk. Check tracking gaps. Review the new terms before 20 Nov.
  - **Framework link:** Rule of 7 (varied touches), STP (angles per segment), Racecar (paid engine fuel = creative + capital).

## 3. Email and SMS
- **2026-11-02:** Gmail, Yahoo and Microsoft all enforce bulk sender rules (5,000+ messages a day): SPF and DKIM, DMARC at least `p=none` with alignment, one-click unsubscribe (RFC 8058) processed within 2 days, and reported spam rate under 0.10% (never reaching 0.30% for Google/Yahoo). Microsoft began rejecting non-compliant mail in May 2025; Google moved to permanent rejections in November 2025.
  - Source: [Red Sift bulk sender guide](https://redsift.com/guides/bulk-email-sender-requirements) `[vendor]`. Confirm with Google, Yahoo and Microsoft sender docs.
  - **Action:** Verify authentication before scaling any flow. Suppress unengaged contacts. Watch spam rate in Google Postmaster Tools.
  - **Framework link:** Rule of 7 and Zeigarnik flows only work if mail lands.

## 4. Legal, trust and compliance
### FTC Consumer Review Rule (US)
- **2026-11-02:** Bans fake reviews and testimonials, sentiment-conditional incentives, undisclosed insider reviews, fake "independent" review sites, review suppression, and buying fake followers or engagement. Civil penalties up to $53,088 per violation (likely higher after 2026 inflation adjustment). FTC sent warning letters to 10 companies and signalled stepped-up enforcement, with supplements, health and wellness, and beauty under closer scrutiny. Brands can be liable for third parties acting for them.
  - Source: [Venable LLP](https://www.venable.com/insights/publications/2025/12/ftc-signals-heightened-enforcement-of-new)
  - **Action:** Review incentives must not depend on positive sentiment. Display reviews honestly. Disclose employee and affiliate connections.
  - **Framework link:** TPB (norms), Brand Resonance (judgements), Pygmalion (no unsubstantiated outcome claims).

### European Accessibility Act (EU)
- **2026-11-02:** In force since 28 June 2025. WCAG 2.1 AA (via EN 301 549) is treated as the practical bar for consumer e-commerce sold into the EU, including non-EU brands. French courts reportedly ordered Carrefour to make its shop and app accessible within six months with daily penalties after; a case against Auchan was decided on procedural grounds and is under appeal.
  - Source: [PinMeTo](https://www.pinmeto.com/news/eu-accessibility-act-enforcement-french-courts-2026/) `[vendor]`, [Bird & Bird (FR)](https://cm.twobirds.com/en/insights/2026/france/accessibilit-numrique--ce-qui-change-pour-les-sites-e-commerce-depuis-juin-2025)
  - **Action:** Run a WCAG 2.1 AA audit for any store selling to EU consumers (contrast, keyboard navigation, alt text, form labels, checkout accessibility).
  - **Framework link:** TPB (perceived control), 4Ps (Place).

## 5. Conversion
- No new primary-source changes logged this week. Use the playbook `playbooks/conversion-audit.md`. Benchmarks vary widely by category and traffic source; do not cite a benchmark without a dated source.

---

## Changelog
| Date | Change |
|---|---|
| 2026-11-02 | Initial seed: Google updates, agentic commerce, Meta, email sender rules, FTC review rule, EAA |
