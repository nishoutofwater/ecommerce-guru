# Playbook: Lifecycle, Retention and Loyalty

**Use for:** email/SMS flows, retargeting, abandonment, repeat purchase, loyalty, referrals, community.
**Frameworks:** Rule of 7 → Zeigarnik → TPB → Brand Resonance → Pygmalion → Racecar (Virality, Lubricants) → Eisenhower.

## Inputs to confirm
- ESP/SMS platform
- List size and consent status by market (ask)
- Repeat rate, time between orders, LTV (ask)
- Product replenishment cycle

## Core flows to check or build
| Flow | Framework hook |
|---|---|
| Welcome series | Rule of 7 (varied touches), TPB (attitude and norms), Pygmalion (identity) |
| Browse abandonment | Zeigarnik, TPB (control: answer objections) |
| Cart and checkout abandonment | Zeigarnik, TPB (control: shipping, returns, payment) |
| Post-purchase / onboarding | Brand Resonance (performance), activation |
| Review request | Brand Resonance (judgements), TPB (norms for future buyers) |
| Replenishment | Zeigarnik, timing to usage cycle |
| Cross-sell / upsell | Decoy, 4Ps |
| Win-back | Rule of 7, Brand Resonance |
| Referral | Racecar virality engine, Pygmalion |
| Loyalty tiers | Zeigarnik (progress), Pygmalion (status), Brand Resonance (resonance) |

## Steps
1. Audit which flows exist and their performance.
2. Map the customer journey touchpoints (Rule of 7).
3. Fill gaps in priority order: cart abandonment, welcome, post-purchase, browse abandonment, win-back, replenishment, referral, loyalty.
4. Check consent and deliverability rules in `best-practices/current.md`. For US SMS, confirm all seven opt-out keywords are honored (FCC rules effective 25 November 2026). For subscriptions sold to UK consumers, confirm reminders, cooling-off notices and online cancellation meet the rules applying from 1 January 2027.
5. Eisenhower sort.

## Output
`templates/audit-report.md` or `templates/growth-plan.md`
