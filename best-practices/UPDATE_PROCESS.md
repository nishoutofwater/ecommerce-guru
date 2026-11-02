# Weekly Update Process

Run every week by a scheduled Claude task. Output is a pull request; nothing merges without review.

## Steps
1. Read `best-practices/current.md` to see what is already logged.
2. Search for changes in the last 7 to 10 days across:
   - Google Search (core and spam updates, AI Mode, Merchant Center, Shopping)
   - AI shopping and agentic commerce (ChatGPT, Google, Perplexity, protocols)
   - Meta, Google Ads and TikTok ad platform changes and policy updates
   - Email and SMS sender rules, deliverability, consent law
   - Consumer protection (FTC, CMA, EU), reviews, pricing, subscriptions, dark patterns
   - Accessibility and privacy law affecting stores
   - Platforms: Shopify, WooCommerce, BigCommerce, payments and checkout
   - Conversion and retention research with real data
3. Prefer primary sources (platform docs and blogs, regulators, courts). Mark vendor sources `[vendor]`.
4. For each real change: add a dated entry under the right section with source link, an **Action** line, and a **Framework link**.
5. Update an existing entry if it changed; do not duplicate.
6. Move entries older than 6 months that are no longer current to `archive.md`.
7. Add a changelog row. Update "Last updated".
8. If nothing material changed, add a changelog row saying so. Do not pad.
9. Write in our own words. Max one short quote per source. No em dashes.
10. Open a PR titled `Weekly best-practices update YYYY-MM-DD` with a 3 to 6 bullet summary.
