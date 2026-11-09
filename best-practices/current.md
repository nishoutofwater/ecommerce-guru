# Current E-commerce Best Practices

**Last updated:** 2026-11-09
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
- **2026-11-09:** The September 2026 spam update ran from 24 September to 8 October, global and all languages. Google did not say what it targeted. As of 2 November no further core update had been confirmed; ranking volatility around 20 to 24 October was reported by third parties and not confirmed by Google.
  - Sources: [Search Engine Journal, spam update complete](https://www.searchenginejournal.com/google-september-2026-spam-update-complete/592283/), [Google Search Status Dashboard](https://status.search.google.com/incidents/XhUDXP7A67iHCD2kmbVu), [Search Engine Roundtable, November report](https://www.seroundtable.com/november-2026-google-webmaster-report-42431.html)
  - **Action:** Compare organic traffic before 24 September and after 8 October before attributing a drop to anything else. Do not attribute late-October swings to a named update.
  - **Framework link:** RACE (Reach), Racecar (SEO engine).

### Agentic commerce (AI shopping agents)
- **2026-11-02:** Two open protocols now let AI agents browse and buy from stores: ACP (OpenAI and Stripe, Sept 2025; see the 2026-11-09 correction on Instant Checkout below) and UCP (Shopify and Google, Jan 2026). Payment layers include Stripe Shared Payment Tokens, Google AP2, Visa Trusted Agent Protocol and Mastercard Agent Pay. WooCommerce, BigCommerce, Wix, Squarespace and others are listed as supporting agentic channels. Consumer trust in letting AI place orders is still low, but AI-referred retail traffic is growing fast.
  - Source: [Search Engine Journal, agentic commerce guide](https://www.searchenginejournal.com/selling-to-ai-the-complete-guide-to-agentic-commerce/)
  - **Action:**
    1. Clean product data: descriptive titles (material, colour, type), complete descriptions, real-time price and stock.
    2. Full Product schema with nested Offer (price, currency, availability, seller) and AggregateRating where reviews exist.
    3. Check platform agentic channel settings.
    4. Test category visibility by asking ChatGPT, Perplexity and Google AI Mode for recommendations.
    5. Track AI referral traffic separately (ChatGPT adds `utm_source=chatgpt.com`).
  - **Framework link:** Racecar (new discovery engine forming), TPB (agents read perceived-control data such as shipping and returns), 4Ps (Place).
- **2026-11-09 (correction):** OpenAI scaled back Instant Checkout in March 2026. Its spokesperson said checkout is moving to Apps and that it is prioritising search and product discovery. ACP continues. Do not plan around native ChatGPT checkout; treat ChatGPT as a discovery channel unless the brand has a ChatGPT app. Reported guidance (based on a Semrush guide, not OpenAI documentation) is that ChatGPT shopping depends on price and product details being in server-rendered HTML, and that OpenAI's search crawlers should be allowed separately from GPTBot, which is used for training. ChatGPT shopping is reported as US only.
  - Sources: [Digital Commerce 360, March 2026](https://www.digitalcommerce360.com/2026/03/06/openai-shifts-checkout-plans-agentic-commerce-strategy/), [StartupHub.ai, 6 Nov 2026](https://startuphub.ai/ai-news/artificial-intelligence/2026/chatgpt-shopping-runs-on-raw-html-now) `[vendor]`
  - **Action:** View source on a product page and confirm price, stock and specs appear without JavaScript. Allow OAI-SearchBot and ChatGPT-User in robots.txt, and decide on GPTBot separately. Check feed values match the product page.
  - **Framework link:** 4Ps (Place), Racecar (discovery engine), TPB (perceived control).
- **2026-11-09:** Google launched Universal Cart in US Search and the Gemini app on 15 October 2026. It runs on UCP, holds items from several merchants in one cart, tracks price changes, applies promo codes and supports Google Pay. Named merchants include Nike, Sephora, Target, Walmart and many Shopify stores. No merchant requirements were stated in the coverage reviewed.
  - Source: [Search Engine Roundtable, 15 Oct 2026](https://www.seroundtable.com/universal-cart-google-search-42312.html)
  - **Action:** US merchants: confirm UCP eligibility through the platform or Merchant Center. Check that promo codes are ones you are willing to have auto-applied.
  - **Framework link:** 4Ps (Place, Price), Zeigarnik (a persistent cart is an open loop), Racecar (discovery engine).
- **2026-11-09:** Shopify extended WebMCP to checkout on 28 September 2026, so browser-based agents can complete orders, including with Shop Pay, with the buyer's authorization, on eligible stores. Fall '26 Editions added a catalog eligibility check for agent channels and a Business details area for the policy and FAQ facts agents may repeat. App platform deadlines: script tags stop running on storefront pages 1 March 2027; Admin API calls using non-expiring tokens return 403 from 1 April 2027; public apps still using those tokens are delisted from 1 January 2027.
  - Sources: [TechCrunch, 28 Sept 2026](https://techcrunch.com/2026/09/28/shopify-opens-checkout-to-browser-based-ai-agents/), [Anatta, Fall '26 summary](https://anatta.io/blog/shopify-editions-fall-2026/) `[vendor]`, [Shopify changelog, app security review](https://changelog.shopify.com/posts/review-app-access-and-security-information-in-shopify-admin)
  - **Action:** Run the catalog eligibility check. Review Business details for accuracy on shipping and returns. List every app and theme using script tags and ask vendors for migration dates. Use the new Settings > Apps security view to find apps with expiring tokens.
  - **Framework link:** TPB (perceived control), Racecar (lubricants: conversion), Eisenhower (schedule migration before March 2027).

## 2. Paid media

### Meta
- **2026-11-02:** Meta's ranking now relies on AI systems (Andromeda for retrieval, GEM and a Generative Recommender for ranking). Creative quality and diversity now drive targeting in Advantage+; near-identical creatives are grouped and count as one. A Creative Diversity score rates ad sets. Advantage+ Creative now rewrites text in images and generates variants by default, so review auto-enhancement settings. Threads became a default placement in October 2026 (bids can be reduced, not fully removed). Customer Lifecycle Strategy toggle steers spend to new customers. Meta is testing AI-generated landing pages on a small share of impressions, where pixels and GA4 may not fire.
  - Source: [Common Thread Collective, Meta ads changes 2026](https://commonthreadco.com/blogs/coachs-corner/meta-ads-changes-2026) `[vendor]`
  - **Action:** Plan creative in distinct concepts (angles, formats, people), not variations of one shot. Audit auto-enhancement defaults for brand and compliance risk. Check tracking gaps.
  - **Framework link:** Rule of 7 (varied touches), STP (angles per segment), Racecar (paid engine fuel = creative + capital).
- **2026-11-09 (replaces the 20 Nov terms note):** Meta paused its revised Commercial Terms, Product Catalog Terms, Self-Serve Ad Terms and Ad Creative Generative AI Terms. They will not take effect on 20 November and no new date has been given; Meta's notice was reported on 5 November. The March 2024 Commercial Terms remain in force. The paused text included a clause allowing Meta to crawl business websites and a section making advertisers solely responsible for AI-altered ads. The pause covers the contract only; it does not change how Meta's crawlers behave.
  - Sources: [PPC Land](https://ppc.land/meta-halts-its-nov-20-terms-that-would-let-it-crawl-business-websites/), [Relevant Audience, quoting the notice](https://www.relevantaudience.com/meta/meta-pauses-commercial-terms-20-november-2026/) `[vendor]`, [Meta Business Help notice](https://www.facebook.com/business/help/2481113349080785) (confirm directly)
  - **Action:** No action needed by 20 November. Still review Advantage+ auto-enhancements, since the brand carries the reputational and compliance risk of what runs. Watch for a reissued version.
  - **Framework link:** 4Ps (Promotion), Brand Resonance (imagery and judgements).
- **2026-11-09:** From 12 November, Meta's setting "Measure conversions on customer devices" is on by default for eligible pixels. Meta says it is not active for people in the EU and UK. Reported conditions are a pixel installed directly on the page (no iframe or image-only pixel) and a site that requires email or phone login, so guest-checkout stores may not qualify. Meta has not said how consent signals are handled or whether these conversions feed bidding. Reported conversions may rise with no change in sales. Separately, product browsing was auto-enabled on existing ads from 28 October, and creative-level breakdowns launched the same day.
  - Sources: [Meta Business Help](https://www.facebook.com/business/help/4237575203200036) (confirm directly), [PPC Land](https://ppc.land/meta-pixel-will-count-more-conversions-from-nov-12-unless-advertisers-opt-out/), [Relevant Audience](https://www.relevantaudience.com/meta/meta-pixel-measure-conversions-on-customer-devices/) `[vendor]`, [Common Thread Collective](https://commonthreadco.com/blogs/coachs-corner/meta-ads-changes-2026) `[vendor]`
  - **Action:** Before 12 November, record Meta-reported purchases, CPA and ROAS against back-end orders and annotate the date. Keep Pixel and Conversions API in place. Review the setting and consent notices with your privacy adviser. Check whether product browsing suits your landing pages and opt out per ad if not.
  - **Framework link:** RACE (Convert measurement), Racecar (paid engine), TPB (perceived control on landing experience).

### Google Ads
- **2026-11-09:** Automated promotions turned on by default on 12 October 2026: Google scans sites for sales and coupons and can show them in Search and Performance Max, only on campaigns with linked location assets and no promotion asset of their own; it can be turned off at account level. Since 1 October resellers, affiliates and secondary sellers cannot use the brand they sell as their business name. New Dynamic Search Ad campaigns end in January 2027 and remaining ones move to AI Max for Search in February 2027.
  - Source: [Keyword Ninja, October 2026 summary](https://keywordninja.com/blog/google-ads-updates-october-2026) `[vendor]`. Confirm with [Google automated promotions help](https://support.google.com/google-ads/answer/7175034), [business name requirements](https://support.google.com/adspolicy/answer/18287059) and [DSA upgrade post](https://blog.google/products/ads-commerce/dsa-upgrade-to-ai-max-2026/).
  - **Action:** Before peak, decide whether automated promotions are acceptable and turn them off if site promo text could be stale or restricted. Resellers: check business name in Ads. Plan DSA migration for Q1 2027.
  - **Framework link:** 4Ps (Price, Promotion), Racecar (paid engine).

### TikTok
- **2026-11-09:** On 5 October 2026 TikTok announced Buy Direct (in-app checkout), a Shopping Assistant, and access for US advertisers to its ad network of nearly 400,000 outside apps, among other products. Most items had no start date, and no defaults or opt-outs were reported.
  - Source: [PPC Land](https://ppc.land/tiktok-opens-ad-network-of-nearly-400-000-apps-to-us-advertisers/). Confirm details in TikTok's newsroom.
  - **Action:** Do not plan peak budgets around these. If you test the ad network, separate its placement reporting so quality can be judged on its own.
  - **Framework link:** Racecar (paid engine), Rule of 7 (placement variety).

## 3. Email and SMS
- **2026-11-02:** Gmail, Yahoo and Microsoft all enforce bulk sender rules (5,000+ messages a day): SPF and DKIM, DMARC at least `p=none` with alignment, one-click unsubscribe (RFC 8058) processed within 2 days, and reported spam rate under 0.10% (never reaching 0.30% for Google/Yahoo). Microsoft began rejecting non-compliant mail in May 2025; Google moved to permanent rejections in November 2025.
  - Source: [Red Sift bulk sender guide](https://redsift.com/guides/bulk-email-sender-requirements) `[vendor]`. Confirm with Google, Yahoo and Microsoft sender docs.
  - **Action:** Verify authentication before scaling any flow. Suppress unengaged contacts. Watch spam rate in Google Postmaster Tools.
  - **Framework link:** Rule of 7 and Zeigarnik flows only work if mail lands.
- **2026-11-09 (US SMS, TCPA):** FCC 26-67 takes effect 25 November 2026 (47 C.F.R. 64.1200(a)(10)). Businesses may designate exclusive opt-out methods if clearly disclosed. Texters using reply-text as the exclusive method must honor seven keywords: STOP, QUIT, END, REVOKE, OPT OUT, CANCEL, UNSUBSCRIBE. An opt-out from a marketing message still revokes all future marketing texts and calls from that sender; the narrower category-specific treatment applies only to informational messages. Maximum 10 business days to honor, with the FCC seeking comment on seven. Comments are due 25 November, replies 28 December.
  - Sources: [National Law Review, 4 Nov 2026](https://natlawreview.com/article/fcc-adopts-overhaul-tcpa-consent-revocation-rules-revoke-all-narrowed-exclusive-opt), [CommLaw Group](https://commlawgroup.com/2026/fccs-new-tcpa-consent-revocation-rules-on-category-specific-opt-outs/) (Federal Register documents 2026-21821 and 2026-21820)
  - **Action:** Test all seven keywords in the SMS platform before 25 November. Check that a marketing opt-out suppresses all marketing and that transactional texts are kept separate. One-way senders must state replies are unavailable and offer another opt-out. Have counsel confirm any exclusive-method designation.
  - **Framework link:** Rule of 7 (frequency caps and channel limits), TPB (perceived control).

## 4. Legal, trust and compliance
### FTC Consumer Review Rule (US)
- **2026-11-02:** Bans fake reviews and testimonials, sentiment-conditional incentives, undisclosed insider reviews, fake "independent" review sites, review suppression, and buying fake followers or engagement. Civil penalties up to $53,088 per violation ([16 CFR 1.98](https://www.ecfr.gov/current/title-16/chapter-I/subchapter-A/part-1/subpart-L/section-1.98), checked 2026-11-09). FTC sent warning letters to 10 companies and signalled stepped-up enforcement, with supplements, health and wellness, and beauty under closer scrutiny. Brands can be liable for third parties acting for them.
  - Source: [Venable LLP](https://www.venable.com/insights/publications/2025/12/ftc-signals-heightened-enforcement-of-new)
  - **Action:** Review incentives must not depend on positive sentiment. Display reviews honestly. Disclose employee and affiliate connections.
  - **Framework link:** TPB (norms), Brand Resonance (judgements), Pygmalion (no unsubstantiated outcome claims).

### European Accessibility Act (EU)
- **2026-11-02:** In force since 28 June 2025. WCAG 2.1 AA (via EN 301 549) is treated as the practical bar for consumer e-commerce sold into the EU, including non-EU brands. French courts reportedly ordered Carrefour to make its shop and app accessible within six months with daily penalties after; a case against Auchan was decided on procedural grounds and is under appeal.
  - Source: [PinMeTo](https://www.pinmeto.com/news/eu-accessibility-act-enforcement-french-courts-2026/) `[vendor]`, [Bird & Bird (FR)](https://cm.twobirds.com/en/insights/2026/france/accessibilit-numrique--ce-qui-change-pour-les-sites-e-commerce-depuis-juin-2025)
  - **Action:** Run a WCAG 2.1 AA audit for any store selling to EU consumers (contrast, keyboard navigation, alt text, form labels, checkout accessibility).
  - **Framework link:** TPB (perceived control), 4Ps (Place).

### UK subscription contracts (DMCC Act)
- **2026-11-09:** New rules apply to consumer subscription contracts entered into on or after 1 January 2027, brought forward from spring 2027 in August 2026. Draft regulations and guidance are published. Requirements include prescribed pre-contract information shown separately from general terms, renewal reminders, a 14-day cooling-off period after a free or discounted trial ends and on renewals of 12 months or more, and online cancellation for online subscriptions.
  - Sources: [Winston Taylor, 21 Oct 2026](https://www.winstontaylor.com/insights/u-k-s-subscription-contract-rules-take-effect-on-january-1-2027-draft-legislation-and-guidance-published), [Latham & Watkins, 14 Sept 2026](https://www.lw.com/en/insights/New-Requirements-Accelerated-for-UK-Consumer-Subscription-Contracts), [draft regulations](https://www.legislation.gov.uk/ukdsi/2026/9780348287912/contents), [draft guidance](https://assets.publishing.service.gov.uk/media/6acf97da2de3184ccf8b814e/subscription-contracts-rules-guidance.pdf)
  - **Action:** Any brand selling subscribe-and-save or memberships to UK consumers: map checkout, reminder emails, cooling-off notices and cancellation to the draft rules now. Plan for legal review.
  - **Framework link:** 4Ps (Price), TPB (perceived control), Zeigarnik (reminders must be honest, not pressure).

### UK CMA enforcement under the DMCC Act
- **2026-11-09:** A consultancy tally to 19 October 2026 reports 15 open CMA investigations, with drip pricing and fake or misleading reviews as recurring themes, and an April 2026 AA/BSM decision with a £4.2m fine. Check the CMA case pages before citing any case.
  - Source: [Change Allies](https://change-allies.com/insights/cma-enforcement-dmcc-open-investigations-oct2026/) `[vendor]`
  - **Action:** UK-facing stores: show mandatory fees in the headline price and audit review collection and display.
  - **Framework link:** TPB (norms), 4Ps (Price), Brand Resonance (judgements).

### EU Digital Fairness Act (proposal pending)
- **2026-11-09:** Not yet published as of 5 October. The European Parliament Research Service expects the Commission's proposal in Q4 2026, with current information pointing to mid-November. Expected topics include dark patterns, subscriptions, influencer marketing and personalisation. Nothing binds yet.
  - Source: [EPRS briefing, 5 Oct 2026](https://eprs.europarl.europa.eu/contents/publications/EPRS/2026/10/EPRS_BRI(2026)791529.html)
  - **Action:** No change needed yet. Re-check next week. Existing EU rules already reach many dark patterns; see the guardrails in `SKILL.md`.
  - **Framework link:** TPB (perceived control), Decoy (option design must stay honest).

### US state privacy changes in 2027
- **2026-11-09:** Effective 1 January 2027: California AB 566 (browsers must offer an opt-out signal such as Global Privacy Control, and businesses apply opt-outs across linked identifiers), Delaware HB 380 (threshold falls to 10,000 consumers), Oklahoma SB 546, and Louisiana SB 386 (over $25 million annual gross revenue; honor browser or device opt-outs). Alabama HB 351 follows 1 May 2027.
  - Source: [ArentFox Schiff, 28 Oct 2026](https://www.afslaw.com/perspectives/privacy-counsel/new-year-new-rules-state-privacy-changes-taking-effect-2027)
  - **Action:** Confirm the consent banner and tag manager honor Global Privacy Control, and that an opt-out carries across cookie, email and login identifiers. Re-check whether you meet each state's threshold.
  - **Framework link:** RACE (Plan and data quality), TPB (perceived control).

## 5. Conversion and demand data
- **2026-11-09 (forecast, not results):** Adobe forecasts US online holiday spend of $275.1 billion for 1 November to 31 December 2026, up 6.7% year on year. Cyber Monday (30 November) is forecast at $15.1 billion and Black Friday at $12.9 billion. Mobile is forecast at a record 63% of spend from Thanksgiving to Cyber Monday. Peak discounts are forecast at up to 30% off list in Cyber Week, varying by category (electronics 30%, apparel 23%, furniture 18%). Clicks from AI tools to US retail sites are forecast up 130%. BNPL is forecast at $21.3 billion for November and December.
  - Source: [Adobe, Sept 2026](https://news.adobe.com/news/2026/09/adobe-us-holiday-shopping-season-to-hit-record)
  - **Action:** Test mobile checkout before any peak code freeze. Set promotional depth against margin and your own history, using Adobe's category peaks only as context. Track AI referrals as their own channel.
  - **Framework link:** 4Ps (Price), TPB (perceived control), RACE (Convert).
- Use the playbook `playbooks/conversion-audit.md`. Benchmarks vary widely by category and traffic source; do not cite a benchmark without a dated source.

---

## Changelog
| Date | Change |
|---|---|
| 2026-11-09 | Corrected ChatGPT Instant Checkout status and FTC penalty note. Replaced Meta 20 Nov terms note (paused). Added Meta on-device conversions, Google Ads, TikTok, Universal Cart, Shopify agentic checkout and deadlines, FCC TCPA revocation (25 Nov), UK subscriptions (1 Jan 2027), CMA enforcement, EU DFA watch, 2027 state privacy, Adobe holiday forecast. Section 2 renamed Paid media. Lifecycle and growth playbooks updated. |
| 2026-11-02 | Initial seed: Google updates, agentic commerce, Meta, email sender rules, FTC review rule, EAA |
