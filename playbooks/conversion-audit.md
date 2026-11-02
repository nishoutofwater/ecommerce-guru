# Playbook: Conversion Audit (PDP, landing page, cart, checkout)

**Use for:** low conversion, high cart abandonment, new page review.
**Frameworks:** TPB → Zeigarnik → Decoy → Eisenhower.

## Inputs to confirm
- URL(s) or screenshots
- Conversion rate, add-to-cart rate, checkout completion (if available; ask, don't assume)
- Device split
- Traffic source mix

## Steps

### 1. First impression (5-second test)
Can a shopper tell what it is, who it's for, and why it's better?

### 2. TPB scan
| Component | Check |
|---|---|
| Attitude | Benefit-led headline, clear outcome, quality imagery/video, specs, comparison |
| Norms | Review count and recency, UGC, ratings near price, endorsements relevant to the segment |
| Perceived control | Price incl. shipping visible early, delivery date, returns, guarantee, payment options, size/usage guidance, support access, guest checkout |

Mark weakest component first.

### 3. Zeigarnik scan
- Checkout steps and progress indicator
- Saved cart and cross-device persistence
- Abandonment flows (cart, browse, checkout) live and timely?
- Free shipping progress bar

### 4. Decoy and offer scan
- Are bundle or tier options present? Is one clearly the target?
- Is the free shipping threshold set to lift AOV realistically?

### 5. Technical and current-practice checks
Check `best-practices/current.md` for page speed, mobile UX, accessibility, payment methods and checkout norms.

### 6. Eisenhower
Prioritise fixes. Pair each with a test or metric.

## Output
`templates/audit-report.md`
