# GTM Strategy & Success Dashboard (Module 6)

## Get your prior work ready
- **The feature you're launching from your M4 PRD, one feature, not a list:** B2, add the First Consumer Card to the phone wallet (Apple/Google) directly from the approval screen.
- **What your M5 experiment will test your hypothesis, primary metric and ship / iterate rule, the evidence the launch rests on:** Hypothesis: If approved M2-persona cardholders can add the card to their phone wallet from the approval screen, a higher share will add it within [X] days of approval, because the add happens at the moment of highest intent rather than requiring them to find it later.
Primary metric: % of approved cards added to a wallet within [X] days of approval.
Guardrail: [e.g., approval-screen drop-off or support contacts, with a numeric boundary].
Ship / iterate rule: Ship if the lift is at least [MDE] at p < 0.05 and the guardrail holds. Iterate if the lift is positive but below MDE. Stop if the guardrail breaks.
- **Your persona pull your M2 persona, this anchors your audience:** Lena

## Set your goal, then your audience
- **Primary GTM goal awareness · engagement · conversion, pick one:** Conversion
- **Why this goal? what makes this the right goal for this feature right now:** The card is already approved, so reach isn’t the problem and awareness would be the wrong goal. The leak is between approved and activated, and the wallet add is the lowest-friction step toward first use. A cardholder who never adds the card has little reason to transact.
- **Target audience the specific segment your goal implies, be precise:** Approved M2-persona First Consumer Card holders on wallet-capable devices who have not added the card to a wallet within [X] hours of approval. Split into (a) those who saw and skipped the prompt and (b) those who never reached it. Exclude devices that can’t use a wallet, so the denominator isn’t inflated.

## Size your launch
- **Launch tier S (minimal) · M (targeted) · L (multi-channel) · XL (full GTM):** M (targeted, owned-led). Upgrade to L only if the sizing math below justifies paid spend.
- **Justification reach + revenue impact + what silence would risk:** Reach: Every approved cardholder is already a customer with known contact details, so they can be reached directly through owned channels at no media cost.
Revenue impact: Indirect. Revenue = approved volume × wallet-add lift × wallet-to-first-transaction rate × value per active card. Fill in the numbers: [volume] × [lift] × [rate] × [value].
Risk of silence: Without reminders, the lift would come only from the in-flow prompt, and cardholders who skip it would probably never come back to it.
- **Is this a launch or a release? does it need go-to-market, or can it just ship?:** A release plus a lifecycle campaign. It needs messaging and measurement, but not a full go-to-market (no press, no sales launch, no new audience).

## Choose your top three channels and plan assets
- **Channel 1 owned / earned / paid, and why it reaches your audience:** Owned: in-app lifecycle message (day 0 and on next app open). It’s the highest-intent touchpoint, reaching people who are already in the app. It only reaches people who reopen the app, so it needs the others as backup.
- **Channel 2 owned / earned / paid, and why:** Owned: push or SMS (day 1). A wallet add happens on the phone, so a nudge there has the least friction. Check consent, and whether these count as service or marketing messages.
- **Channel 3 owned / earned / paid, and why:** Owned: email (day 3, final reminder day 7). It reaches people who aren’t opening the app. It’s slower, so it works as a follow-up, not a first touch.
- **Enablement & assets what Sales / CS / Support need, plus the assets to build (one-pager, demo, etc.):** Removed from the original plan: Sales-agent word of mouth is untracked, has no owner and is probably absent from a digital approval flow. Treat it as an optional extra, not a channel.
Paid ads would pay to reach people you already can contact. Reconsider only as customer-match retargeting, and only if legal and consent allow it.

Enablement & assets:
Marketing: in-app copy, push/SMS copy, email sequence (3 touches).
Support/CS: help page, a “wallet add failed” troubleshooting script, a short briefing on the feature.
Compliance: sign-off on reminder copy and channel consent.
Analytics: tracking events for approval, prompt shown, wallet add and first transaction, plus the holdout group.

## Make it executable
- **Ownership named owner per key activity, individual, not department:** Feature and instrumentation: [name], PM
Messaging and channel execution: [name], PMM
Support readiness: [name]
Compliance sign-off: [name]
Budget approver: [name]
- **Budget & resource gaps what costs extra, and any asset you can't currently build:** No budget is stated, so confirm it. Owned-only needs mostly internal time, and paid media only if the L upgrade is approved.
Possible SMS per-message costs.
Gaps to confirm: in-app messaging capacity, compliance review time, and whether the tracking events exist today.
- **Timeline Phase 1 beta → Phase 2 launch moment → Phase 3 post-launch:** Phase 1, Beta ([dates]): Run the M5 experiment with a holdout group. Test the in-app and push copy.
Phase 2, Launch moment ([date]): Release the feature and start the reminder sequence for new approvals. Depends on [engineering release] and Apple/Google readiness.
Phase 3, Post-launch (day 7 and day 21): Day 7 is the early check, and day 21 is the scale/hold/retire decision.

## Define how you'll know it worked
- **Success metrics 2 to 3 metrics that match your GTM goal:** Primary: Wallet-add rate within [X] days of approval: [baseline]% → [target]% by day 21, measured against the holdout group. Your brief said “+20p”. I’ve assumed this means a lift in percentage points, but please confirm it, since +20 points and +20% are very different targets.
Outcome: Wallet-to-first-transaction rate, because your goal is activated cards, not wallet adds.
Guardrail: [support contacts or approval-flow completion], with a boundary of [X].
- **Bad signal to watch for e.g. high reach, zero signups = message-market mismatch:** At day 7, the wallet-add rate is less than [baseline + Y points] above the holdout. This is actionable. First check the approval-screen flow (is the prompt shown and tapped?), then message performance (opens and clicks). High prompt taps with low completed adds points to a technical or wallet-provider problem, not a messaging one.
- **Most likely post-launch decision double-down · iterate · pivot · deprioritize, and what would trigger it:** Double-down (add paid or an L tier): the day-21 lift meets target and wallet-to-transaction is healthy.
Iterate: the lift is positive but below target, so rework timing and copy.
Deprioritize reminders: the in-flow prompt alone captures most of the lift, so the reminders add little.
