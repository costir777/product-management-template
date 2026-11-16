# Increasing the cards activation rate by boost the ratio of cards added to wallet

> Easy to pay by wallet, easy to use your new Riverty card

**Costi Rantz | Cohort 2 November 2026** · https://github.com/costir777/product-management-template

Prototype: https://github.com/costir777/product-management-template/blob/main/04-roadmap/prototype.html.html

---

## Final Project Deliverables

### Slide 5 · Strategy
- **Problem:** ## Responses
- **Chosen path, which Riverty business-unit case are you using?:** BU Pay & Credit
- **Strategic crisis, based on the brief, if the company does nothing for 12 months, what happens to its market position?:** What I’d expect after 12 months of doing nothing (my inference)

The new bank has no consumer proposition to differentiate it. The licence is a cost and a promise to the group. Without a card or similar product, the consumer-finance growth story rests on checkout volume alone.
Riverty stays invisible to consumers. It is branded behind merchants, so shoppers have no direct relationship with it. Riverty’s own research notes that wallets strengthen Apple, Google or Samsung rather than merchants. A competitor that owns the consumer’s wallet can steer where people pay later. 
riverty
A year of learning is lost. There would be no data on who uses a card, what it earns, or how it affects merchants. The next move would then be a larger and riskier bet. German card issuing is also getting cheaper to enter, with Nexi and Visa offering banks a faster, lower-cost route to launch cards, so the window for a first-mover advantage narrows. 
pulse
- **Moment of misery, what is the user likely doing outside the product (Google, spreadsheets, a competitor) because your tool isn’t serving them?:** Adding up what they owe by hand without Riverty but with other providers.
- **Problem hook, summarize the business risk and user pain into one urgent sentence.:** Riverty’s card is losing about a quarter of approved users before activation and a third of activated cards before wallet add, while users who can’t see what they owe or why a payment was declined fall back on their bank card.
- **Value proposition, based on the initiative in your assigned Riverty case, what is the new value and why is it urgent to launch now?:** New value: a pay-later card for heavy BNPL users that works beyond checkout. It shows one clear balance, one due date and a reason for every decline. Partner-merchant offers would route spend back to Riverty’s merchants rather than to big marketplaces.

Why now:

The bank is ready. Riverty’s Luxembourg banking licence was scheduled to begin operations in July 2026, and coverage says it will expand consumer finance with new products. A bank without a consumer product to differentiate it is a cost without a story. 
thepaypers
it-finanzmagazin
The window is narrowing. Nexi and Visa are giving German banks a faster, lower-cost way to launch cards, and Riverty’s own research notes that wallets strengthen Apple, Google or Samsung rather than merchants. Whoever owns the consumer’s wallet steers where they pay later. 
pulse
riverty
Changes take months. Ops says (N-11) that any proposition change goes back through approval for pricing, credit policy and terms, so the learning has to start before the bigger decisions.
The fixes are cheap. In the fictional test data, the biggest losses are fixable: 155 approved people never activate, and 143 cards never reach the phone wallet. Heavy users already activate at 82.6%, so the proposition works when the basics don’t fail.

One-line version: launch a small, fixed MVP now to learn what a Riverty card is worth before cheaper competitors and wallets lock in the relationship.

The “now” argument rests on public reporting and my own reasoning, and the data points come from the fictional pack. I’d treat any claim that a competitor card already exists in Germany as unchecked.

## Cold-read your own hook
- **Is the business risk high enough to justify a new initiative, a high-stakes threat, or a minor inconvenience?:** Verdict: it justifies a small, bounded initiative, but it isn’t yet a high-stakes threat. I’d call it a moderate, slow-building strategic risk, with a cheap way to test it.

Why it’s more than an inconvenience

Riverty has a banking licence and said it will expand consumer finance, so it has to show a consumer story.
Wallets and cheaper card issuing narrow the window for owning the consumer relationship.
The pilot shows concrete leaks: 155 approved users never activate, 143 cards never reach the wallet, and 8.7% of in-store payments are declined with no reason shown.

Why it isn’t a high-stakes threat

Riverty’s core checkout BNPL business is strong and growing. Nothing here suggests it is losing volume today.
The cost of waiting is erosion, not a crisis. It’s a loss of options over 12 months, as I argued earlier.
The pilot is tiny (1,200 invitees, 253 of them active cards) and flattering. 639 of the invitees are employees, so the numbers likely run high.

What I can’t verify

I have no data on Riverty’s market share or on competitor cards in Germany, and the pack’s figures are fictional. The risk rating rests on reasoning, not on measured loss.

So the right size of response is the MVP. It costs little, and the downside of being wrong is small. If the test shows a heavy-user segment that keeps using the card and merchants that gain from it, the case becomes much stronger. If not, you’ve spent very little to find that out.
- **Is the moment of misery a systemic problem or just an edge case?:** Mostly systemic. The core pain comes from how the product is built and set up, not from rare situations.

Systemic

Two places to look, two due dates (T-103, T-104, N-07). The card and pay-later orders are separate products, so anyone with both hits this. It’s a design problem, not a glitch.
Wallet add (T-102). 33.2% of activated cards (143) never reach the phone wallet. Online purchases don’t need it, but in-store use does, and in-store use is what makes this a card rather than a checkout option.
Activation leak. 26.5% of approved users (155) never activate. At that scale it’s a pattern in how people are onboarded, not a few unlucky cases.
Declines with no reason (T-101, N-06). The 8.7% in-store decline rate is the visible part. The gap is systemic because the app explains none of them.

Closer to edge cases

The identity-check re-upload loop (T-106), late push notifications in some shops (T-108), and instalments appearing only for some categories (T-105) are narrower and more bug-like. They still cost trust, but they’re a smaller share of users.
The missing credit-score article (T-107) hits everyone who wonders, but it’s cheap to fix.

Caveats

In-store is only about 17% of purchases, so decline pain is concentrated in one use case.
The pack has 8 tickets and 12 interview notes, which show patterns but not how many people are affected.
With 53% of invitees being employees, real customers probably see worse numbers (N-10).

To confirm, I’d check how many people hit more than one problem. If the same users get declined, can’t see their total and get double reminders, the problem is systemic. If each issue hits a different small group, it’s closer to a set of separate bugs.
- **Does the value proposition actually remove the obstacle you identified, or is it a generic feature?:** Partly. The specific pieces remove real obstacles, but the headline proposition (“a pay-later card that works beyond checkout”) is generic, and the card form is what creates the friction.

Specific, and tied to a named obstacle

One balance and one due date (B3, B8) answer the moment of misery directly: adding up what they owe by hand (N-07, T-103, T-104). Of everything in the proposition, this is closest to a real differentiator, because it only works if the card and Riverty’s pay-later orders sit together.
Decline reason (B1) and wallet add (B2) remove named leaks (T-101, T-102).

Generic or unproven

“Works beyond checkout” doesn’t solve any observed pain. N-02 says a third app is one more thing to check, and N-03 says they tap their bank card without thinking. Being accepted everywhere doesn’t give a reason to choose it.
Partner offers (B5) answer the merchant’s question (N-08), not the user’s pain, and N-09 is only conditionally interested.
Fixing bugs isn’t a value proposition. B1 and B2 make the card work as expected, but the card still has to give users a reason to pick it.

Gaps

Nothing in the proposition targets the 155 approved users who never activate. We don’t know why they stop.
Showing a decline reason explains declines but doesn’t reduce the 8.7%.
B8 touches pricing, credit policy and terms, so by N-11 it may not fit an MVP.

A sharper version: “One total and one due date for everything you pay later, in the card you already have to carry.” It is aimed at heavy BNPL users, ties to the misery moment, and is something a bank card or wallet can’t copy easily.

To test it: ask heavy users in the pilot whether one total and one due date would make them use the card instead of their bank card, and compare against a group that gets only the bug fixes.
- **Value proposition:** Make consumers love the new Riverty card and use it top of wallet
- **Hypothesis:** ## Pre-work · Hypothesis check
- **Role , who you are solving for (from M2):** Product Manager
- **Goal , what this user is ultimately trying to achieve:** launching first Riverty consumer card
- **Friction / moment of misery , the specific pain blocking their goal:** Riverty lacks a consumer card, which would allow users to pay anywhere also in stores
- **Current workaround , the external tool or manual process they rely on (M2):** No consumer cards yet
- **Problem Hook , your one-sentence framing of the business crisis (M1):** No consumer card, no stickiness from users and lost usage
- **Value Proposition , the outcome your initiative promised to deliver (M1):** Driving Riverty consumers to boost their usage and loyalty

## Read the evidence in your case
- **Where does your case say people stall or leave? Does that match the friction you wrote in Module 2?:** The biggest problem is the very first step: invited → applied. Only 59.7% apply, so 484 people (40.3% of everyone invited) drop out before they even start. That is the largest absolute loss in the funnel and the largest single drop in conversion.
- **What got better or worse in the case, and does that support the workaround your persona uses?:** With Month 4 complete, the picture is less rosy than my earlier read. Several things I called improvements reversed in Month 4.

Got better

Spend per active card: €200 → €233 (+17%). Purchases per card also crept up (3.8 → 4.2), and the average purchase value rose to about €55 in Month 4, from about €51 in Month 3. Volume is still growing (+3.8% in Month 4) even with fewer cards.
Overall scale: Volume is about 4x Month 1 (€15.2k → €61.1k), and active cards are 3.4x.
In-store declines vs Month 1: 8.7% is still well below the 12.1% starting point, even after the Month 4 rebound.

Got worse

Declines are at their pilot high. The overall decline rate went 2.7 → 2.2 → 2.6 → 3.5%, so Month 4 is the worst month, and the trend has been up since Month 2.
In-store declines reversed. They fell from 12.1% to 6.4% by Month 3, then jumped to 8.7%. I called this the clearest improvement last time, but that improvement didn’t hold.
Online declines likely rose too. By my rough back-calculation (in-store is about 17% of purchases), the implied online decline rate moved from about 1.8% to about 2.4%. That is an estimate, since the rates may not share the same denominator, but it suggests the problem isn’t only in-store.
Active cards and purchases fell in Month 4 (278 → 262 cards, -5.8%; 1,162 → 1,107 purchases, -4.7%). This is the first shrinkage in the pilot.
Instalments share slipped from 18.1% to 17.4%, so my earlier “steadily climbing” no longer holds.

Flat or unclear

In-store share of purchases has stayed in a 15-18% band, so usage remains mostly online.
Partner merchant share of volume bounced between 57% and 63% (63.1% in Month 4). That is noisy rather than a trend.

How to read it: Month 4 looks like a quality-and-retention warning. Fewer cards are active, and the rise in spend per card may partly be survivorship: lighter users drop out, which lifts the average. At the same time, more transactions are being declined. A higher decline rate could itself be driving the drop in active cards, because people who get declined tend to stop using the card. That fits the funnel, where only 72% of first-time buyers reached 3+ purchases. I can’t prove the causal link from this data.

The most useful next step would be the decline reasons (insufficient limit, risk rules, merchant category, technical errors) split by month, to see what changed in Month 4. It is only one month, so I’d treat it as a signal to investigate rather than a confirmed trend.
- **Which user in the case is carrying the pain, and is that the person your Module 2 persona describes?:** Short answer: the light BNPL user is carrying the most pain in this data. I can’t check whether that matches your Module 2 persona, because I haven’t seen it in this conversation. If you paste it, I’ll compare directly.

Why light BNPL users

They drop out at activation most. Only 62.0% of approved light users activate, against 74.7% for regular and 82.6% for heavy. That is 60 of 158 approved people (38%) who were approved and never switched the card on. This is the same approved → activated leak that showed up in the funnel.
They barely use the card once active. They make 2.46 purchases per active month, against 5.82 for heavy users, and spend about €125 a month, against €321.
They skew in-store. 24.5% of their purchases are in-store, against 12.1% for heavy users. In-store was where declines were worst in the trend (8.7% in Month 4, versus 3.5% overall), so light users are probably the most exposed to declines. The user split has no decline rate by segment, so this is an inference, not something the data shows.
They don’t use instalments. Only 6.0% of their purchases are instalments, against 25.4% for heavy users. The card isn’t doing a job they need.

Other segments

Regular users lose the most people in absolute terms at activation (66 of 261 approved), but at a rate close to the funnel average.
Heavy users are the healthiest, but they matter most for volume. They lean on partner merchants (68%) and instalments, so any decline problem there would hurt revenue most. I can’t see that from this data.
Age and relation (employee vs friend or family) show only small differences. Activation ranges from 71% to 81% across age bands, and the 45-54 band is highest. Those aren’t where the pain is.

Caveat: the invited pool is only employees and friends or family, so this is a friendly, non-representative group. Light users here might behave differently from light BNPL users in the general public.

To compare with your Module 2 persona: check whether it describes someone who is occasional or sceptical about BNPL, shops more in-store, and is less interested in instalments. If your persona is a frequent, instalment-driven shopper, it describes the heavy user, who is the healthiest group here, not the one in pain.

## Step 2 · Craft your hypothesis
- **Qualitative evidence (from M2) , quote the specific friction / moment of misery for your persona:** Here is the completed table. I chose the moment where the funnel, user split and notes all point the same way, and I flag below where the evidence is thinner.

Field	Entry
Moment	Approved, but never activates the card (approved → card activated)
User	Light BNPL user: occasional, more in-store, rarely uses instalments
Funnel evidence	73.5% of approved people activate, so 155 of 586 are lost. This is the largest leak among people who already said yes.
User split evidence	Light users activate at 62.0% (60 of 158 approved people never do), against 74.7% for regular and 82.6% for heavy users. Once active, they make 2.46 purchases a month (heavy: 5.82) and use instalments in only 6.0% of purchases.
Trend evidence	Overall declines peaked at 3.5% in Month 4, and in-store declines rebounded to 8.7%. Light users are the most in-store segment (24.5%), so they are probably the most exposed. That is an inference, since declines aren’t split by segment.
Qualitative evidence (from M2)	N-05, light BNPL user, 45-54: “A credit card with interest is exactly what I try to avoid. If it says instalments I get nervous.” It is backed by T-107: participants ask whether the card affects their credit score, and no help article exists.

Hypothesis:

We believe that light BNPL users are approved but don’t activate or keep using the card because they read it as a credit card with interest, and the app gives no reassurance (no clear cost, no credit-score answer), which makes them nervous about turning it on. We see this in the data as a 62.0% activation rate against 82.6% for heavy users, and 2.46 purchases per active month against 5.82. If we add a plain-language “what this card costs and what it doesn’t do” step, including the credit-score answer, to the approval and activation screens, we expect activation among light users to rise from 62.0% toward the regular-user level (about 75%), and we’d know it worked if approved → activated for light users reaches 70% or more within the next invitation cohort.

Where the evidence is weak:

It’s one quote. N-05 is a single interview, and the 45-54 band actually activates best (81.2%), so the quote doesn’t line up neatly with the age data. Treat it as a lead, not proof.
The data doesn’t say whether the card carries interest. I wrote the cause as what the user perceives, which is all N-05 supports. If the card has no interest, that makes the fix cheaper, because it is a messaging problem.
The trend link is the weakest part. The decline data isn’t split by segment, so it only loosely supports this moment.

A stronger alternative if you’d rather follow the trend data: the post-activation moment, “declined in store with no reason shown” (N-06, T-101, T-102). It has a vivid quote, 48 in-store declines in the log, and 143 activated cards that never reached the phone wallet. It also fits the Month 1 cohort, where only 66.3% were still active a month later. But it isn’t specific to light users, and it’s about retention rather than activation. If you pick it, the user changes to anyone who pays in store, and the metric becomes the in-store decline rate (8.7% baseline) or one-month retention.
- **Quantitative evidence (from M3) , name the metric or data point that confirms the pain; cite the number:** The metric that confirms the pain is the approved → activated rate for light BNPL users: 62.0%.

The number to cite: 98 of 158 approved light users activated, so 60 people (38.0%) were approved and never switched the card on. The comparison points are 74.7% for regular users and 82.6% for heavy users, and 73.5% overall (431 of 586) in the funnel and baseline table.

Supporting numbers, if you want a second line:

Usage after activation: light users make 2.46 purchases per active month, against 5.82 for heavy users, and spend about €125 a month, against €321.
Size of the gap: if light users activated at the regular-user rate (74.7%), about 20 more of the 158 approved would have activated (118 vs 98). That is a rough sizing, not a forecast.

Suggested entry for the table:

Approved → activated is 62.0% for light BNPL users (98 of 158), versus 74.7% for regular and 82.6% for heavy users, and 73.5% overall (431 of 586).

Two cautions on how far this number goes:

It confirms where the pain is, not why. The 62.0% shows light users stall at activation. The interest and credit-score reading comes from N-05 and T-107, not from the data.
The sample is friendly. N-10 notes the test group is mostly colleagues, so the real rate for the general public could be lower. Employees activated at 71.9% and friends or family at 76.1%, so the pool isn’t uniform either.

If you’d rather anchor on the trend moment instead (in-store declines), the number to cite would be the 8.7% in-store decline rate in Month 4 (up from 6.4% in Month 3, base of 206 in-store attempts). I’d keep the activation metric, since it matches the persona and moment you’ve chosen.
- **Persona , role, goal, and the friction you confirmed in the reconciliation steps:** Here is the persona entry. The role and friction are grounded in the data and notes. The goal is partly my inference from one quote, and I mark it as such.

Field	Entry
Persona	The cautious occasional pay-later user (a composite built from N-05 and the light segment, not a real person)
Role	Consumer, light BNPL user. Invited as an employee or friend/family in the test launch, approved, but one of the 60 of 158 approved light users who never activated. N-05 is in the 45-54 band.
Goal	Pay for everyday purchases without taking on interest or debt they didn’t plan for. In N-05’s words, a credit card with interest is “exactly what I try to avoid.” They want a clear answer on what it costs before they commit.
Friction confirmed	The card looks like a credit product, and the app doesn’t reassure them. They get nervous at the word “instalments” (N-05) and have no answer on whether the card affects their credit score (T-107, no help article). They approve but don’t switch it on.

How each snapshot confirms the friction

Funnel: approved → activated is the largest leak among people who already said yes (73.5%, 155 of 586 lost).
User split: light users activate at 62.0% (98 of 158), against 74.7% for regular and 82.6% for heavy users. Those who do activate use it little: 2.46 purchases a month, about €125 spend, and instalments in only 6.0% of purchases. This fits someone who doesn’t want the credit-like feature.
Trend: this is the weakest confirmation. Light users are the most in-store segment (24.5%), and in-store declines rose to 8.7% in Month 4, so they may be more exposed. But declines aren’t split by segment, so I’d call it supporting context only.

What to be careful about

The goal is inferred. N-05 supports “avoid interest” directly. “Wants a clear cost answer” is my reading of that quote plus T-107.
The age detail doesn’t fit neatly. The 45-54 band activates best (81.2%), so I’d define the persona by BNPL usage, not age. If you keep an age, say it comes from a single interview.
It rests on one interview and one ticket. If you have other light-user quotes in your Module 2 work, add them to strengthen this.

One-line version for the table:

A cautious occasional pay-later user who wants to avoid interest and debt, approved for the card but unsure what it costs or whether it affects their credit score, so they never activate it.
- **Problem you are solving , one sentence describing the specific friction this initiative removes:** Problem statement:

Light BNPL users who are approved for the card don’t activate it because nothing in the app tells them what it costs or whether it affects their credit score, so a card they read as “credit with interest” stays switched off (62.0% activate, against 74.7% for regular users).

Shorter version, if the field is tight:

Approved light BNPL users are unsure what the card costs and whether it affects their credit score, so 38% of them never activate it.

What each part rests on:

“Don’t know what it costs / credit score”: N-05 (nervous at “instalments”, avoids interest) and T-107 (credit score question, no help article).
The number: 98 of 158 approved light users activated, so 60 (38.0%) did not.

One thing to keep honest: the sentence names a cause (unclear cost and credit-score impact) that comes from one interview and one ticket, not from the activation data. If your reviewers push on it, the safe wording is “appear to” or “are likely to” before “don’t activate,” and a quick check with a few light users who never activated would confirm it.
- **Strategic outcome , what behaviour change do you expect, and how does it map to retention / revenue / churn?:** Strategic outcome:

More approved light BNPL users switch the card on and use it as an everyday payment option, because they know what it costs and that it doesn’t hurt their credit score. This turns approved-but-dormant cards into active ones.

Behaviour change we expect

	Today	Target
Light users who activate once approved	62.0% (98 of 158)	70% or more, stretch 74.7% (the regular-user rate)
Light users who then make a first purchase	Not split by segment (overall 81.2% of activated)	At least the overall rate
Light users who keep using the card	Not measured for this segment	Same retention as other activated cards

The behaviour change is a decision at the approval screen. People who got approved and stalled now turn the card on, and what follows depends on whether they find a reason to use it.

How it maps to retention, revenue and churn

Lever	Link	What the data supports
Activation (the direct effect)	More approved people become cards in use	At 70%, about 13 more of the 158 approved light users activate (111 vs 98). At 74.7%, about 20 more.
Revenue	Each active light card brings card volume	A light user spends about €125 a month, about €1,500 a year if that held. So the 13 to 20 extra cards add about €1,600 to €2,500 in monthly volume in the pilot. This is volume, not revenue. The pack has no interchange or fee rate, so you need to state your own take-rate assumption.
Retention	Only helps if the new users stay	Activated cards drop off fast. Of the Month 1 cohort, 77.6% bought in month 0, 66.3% in month 1 and 51.0% in month 2. Light users already use the card least (2.46 purchases a month), so the extra cards are likely the least sticky.
Churn	Weakest link	Annual churn isn’t measurable in four months, per the data pack, so you have to state an assumption. Activating a card prevents a dormant card from being abandoned, but it doesn’t reduce churn by itself.

Conservative sizing: per 100 approved light users, the target adds 8 activations at 70% (about 13 at 74.7%). Because only about 75 to 85% of activated cards buy in their first month, expect somewhat fewer actually active cards than that. Scale it to your assumed audience only if you state what share of the base is light users. The pack gives none. In the pilot it was 354 of 1,200 invited (29.5%).

What I’d write in the table:

Outcome: more approved light BNPL users activate and use the card. Activation moves from 62.0% to at least 70%, which adds active cards (about 13 per 158 approved light users) and card volume (about €125 a month each). The retention and churn benefit depends on those users staying active past month 2, which we will track.

Where this claim is limited

Activation is not retention. If the intervention only gets people to activate, the extra cards may go quiet by month 2 like the others. Add a retention metric, such as the share of newly activated light users who purchase in month 1, so the outcome isn’t claimed on activation alone.
Revenue is volume. Don’t present €1,600 to €2,500 a month as income without a take-rate assumption.
The pilot is friendly. N-10 says the test group is mostly colleagues, so real-world activation and spend are likely lower.
Churn is an assumption. If you need one, label it as yours, for example “assume X% annual churn for light users”, and show how a retained card changes the lifetime volume.

If you give me a take-rate and an assumed churn figure, I can turn this into a simple per-100-users value estimate.
- **Primary success metric (initiative signal) , the leading indicator that tells you the gap is closing:** Primary success metric:

Approved → activated rate for light BNPL users. Baseline 62.0% (98 of 158). Target 70% or more, stretch 74.7%.

Why this is the right leading indicator

It’s the gap itself. The pain moment is “approved but never activates,” so the metric measures that step directly, and it moves quickly. You see it within one invitation cohort, without waiting months for churn or revenue.
It’s already measured. The funnel, user split and baseline table all use the same definition (activated cards divided by approved people), so you can compare before and after without building anything new.
It sits upstream of retention and revenue. An approved person who never activates can’t buy, so every later outcome depends on this step.

How to write it in the table

Field	Entry
Metric	Approved → activated rate, light BNPL users
Baseline	62.0% (98 of 158 approved), against 73.5% overall
Target	70% or more within the next invitation cohort
Window	Activation within 30 days of approval (the pack doesn’t state a window, so define it and keep it the same before and after)
Signal that the gap is closing	Light-user rate moves toward the regular-user rate (74.7%)

Guardrails to track beside it

These stop you from claiming a win on activation alone:

First purchase within the activation month for newly activated light users. Baseline is 81.2% overall, and it isn’t split by segment, so you need to measure the light-user baseline first.
Purchases per active month for light users (2.46 today). If activation rises but this falls, the extra cards are dormant.
Overall decline rate (3.5% in Month 4), so a rise in activations doesn’t hide a worsening payment experience.

Cautions

Sample size. With 158 approved light users, a few people move the rate by several points. Going from 62.0% to 70% means about 13 more activations, and a sampling swing of that size is plausible. Use a larger cohort, or treat a small uplift as directional only.
Friendly pool. N-10 says the test group is mostly colleagues, so the baseline may be flattering. Compare against a control group (same approved light users without the new screens) if you can.
Attribution. Other changes in the same period, such as the wallet fix (T-102), could move activation too. Change one thing at a time, or note what else shipped.

If you want, I can turn the metric, guardrails and thresholds into a one-line success criterion for the hypothesis sentence.
- **Guardrail metric (product signal) , the metric that must NOT drop; it protects your existing base:** Guardrail metric:

Approved → activated rate for regular and heavy BNPL users (the healthy core). Baseline 77.8% combined (333 of 428 approved): 74.7% for regular, 82.6% for heavy. It must not fall below the floor.

Why this protects the existing base

The fix touches everyone. A “what this card costs and doesn’t do” step on the approval and activation screens is seen by all approved users, not only light ones. If the added reassurance makes heavy and regular users hesitate, or adds friction to a step they already pass easily, you would gain activations from light users and lose them from the people who carry the volume.
They are where the volume is. Heavy users make 5.82 purchases per active month and spend about €321. Regular users make 3.91 and spend about €200. Together they are 333 of the 431 activated cards (77%).
It uses the same definition as your primary metric, so the before and after comparison needs nothing new.

How to write it in the table

Field	Entry
Metric	Approved → activated rate, regular and heavy BNPL users combined
Baseline	77.8% (333 of 428), with heavy at 82.6% and regular at 74.7%
Floor	Must not drop below about 74% in the test cohort. This is my suggested threshold, not from the pack. Set your own, and the same window as the primary metric.
If breached	Pause the rollout and check whether the new screens add friction for users who didn’t need them

Backup guardrails

Overall decline rate stays at or below 3.5% (Month 4 baseline). It protects the payment experience as activations grow.
Purchases per active month for heavy users stays at or above 5.82, so the screens don’t change how the best users behave after activating.

Limits to flag

The pack has no data on existing pay-later usage. The guardrail that would best protect the established BNPL base, such as regular pay-later orders or repayment behaviour per user, isn’t there. N-07 and T-103/T-104 show the card and normal pay later already confuse people, so if you can get that measure, add it. Otherwise say it is not measurable in the pilot data.
Noise. With 428 approved users, a few people move the rate by a point or two, and the sampling swing is probably around ±4 points. A small dip below baseline is not by itself a breach, so define the floor with that in mind.
Friendly pool. N-10 says the test group is mostly colleagues, so the baseline may be flattering.

If you want, I can combine the primary metric, this guardrail and the thresholds into one success criterion for the hypothesis sentence.
- **Decision window , how much time or data before you scale, pivot, or kill? minimum threshold to proceed?:** Decision window:

Read the result once at least 280 approved light users have had 30 days to activate. Check the retention guardrail at 60 days. Decide at that point, not earlier.

Data needed

Item	Number	Basis
Approved light users, before/after against the 62.0% baseline	about 280	Standard calculation to detect 62% → 70% (80% power, 95% confidence). It is my estimate, not from the pack.
Approved light users per arm, with a control group	about 550 each (1,100 total)	Same calculation, comparing two groups
Invitations needed	about 2,100 (before/after), about 8,300 (with control)	In the pilot, 158 of 1,200 invited (13.2%) became approved light users
Why not the pilot size	158 gives a ±7.6 point margin on 62.0%	The target gain is 8 points, so the pilot can’t tell a real lift from noise

The larger sample means a control group is expensive at pilot scale. If you can’t get it, use before/after and note what else shipped (T-102 wallet fix, for example).

Time needed

Day 30 after approval: activation read (primary metric).
Day 60: share of newly activated light users who purchased in month 1. Overall cohorts retained 64-69% at month 1 and 51-57% at month 2, so this shows whether the new activations are real or dormant.
Don’t wait for churn. The pack says annual churn can’t be measured in four months, so label it an assumption.

Decision rules

These thresholds are my suggestions, so set your own.

Decision	Condition (at 280+ approved light users)
Scale	Light activation ≥70%, and the lower end of the 95% range is above 62%. Guardrails hold: regular and heavy activation ≥74%, decline rate ≤3.5%, heavy purchases ≥5.82. Month-1 purchasing among new light activators is at least about 64%, the overall month-1 rate.
Keep running	Activation 65-70%, or sample not reached. The result is positive but not proven, so don’t decide yet.
Pivot	Activation under 65% with the full sample, or activation rises but month-1 purchasing falls (cards switched on but unused). The cost/credit-score cause is probably wrong. Interview light users who never activated, then consider the in-store moment instead (N-06, T-101, B1).
Kill	No lift (about 62% or lower) with the full sample, or a confirmed guardrail breach that persists after a fix.

Minimum threshold to proceed: light-user activation of at least 70% on at least 280 approved light users, with no guardrail breach. Below that, don’t scale.

Things to plan for

Approval lead time. N-11 says proposition changes go back through pricing, credit-policy and terms approval, which takes months. A cost and credit-score explanation may need legal or compliance review even if the terms don’t change, so build that time into the start date.
Friendly pool. N-10 says the test group is mostly colleagues. If the real activation baseline is lower, the 70% target may be too easy, so re-measure the baseline in the new cohort before judging.
Light users are a small slice. At about 13% of invitees, reaching 280 takes a larger invite wave than the pilot. If that isn’t possible, extend the window rather than loosening the thresholds.

I can combine the hypothesis, metrics, guardrail and these rules into one summary block for your submission.
- **Draft your full hypothesis sentence , one to three sentences; quote the metric, name the persona, name the outcome:** Based on N-05 and T-107 and a 62.0% light-user activation rate (against 74.7% for regular users), I believe that explaining what the card costs and that it doesn’t affect credit scores for cautious occasional pay-later users will lift their approved → activated rate from 62.0% to at least 70%. I will protect regular and heavy users’ activation (77.8%, floor about 74%) and make a go/no-go decision after 280 approved light users have had 30 days to activate.

### Slide 6 · Research
- **Competitive analysis:** ## Responses
- **Role, who are you solving for? (the specific user segment or profile):** Persona 1: Lena, the Heavy Pay-Later Juggler (from your brief; 25-34 heavy-user profile, N-01, N-02)

Role: A 32-year-old salaried Cologne shopper with no financial cushion who uses BNPL on most non-trivial purchases and takes whichever of Klarna, PayPal or Riverty appears at checkout.
- **Goal, what is this user ultimately trying to achieve?:** To keep money in her account until she has decided to keep the item, without losing track of what she owes before payday.
- **Friction, the main barrier (moment of misery) stopping them from succeeding:** Friction: She adds up what she owes by hand across providers, and a Riverty card would be “one more thing to check before payday” (N-02), while the card and Riverty’s own pay-later orders already sit on separate screens with separate dates (N-07, T-103, T-104).
- **External tools, the outside platforms or tools the user is forced to use:** Klarna, Paypal and her manual ways to keep track of total amounts due and timelines, by provider
- **The process, the 3 to 5 manual steps the user takes to get the job done:** Steps

Choose at checkout. She uses whichever BNPL option appears (brief). Evidenced.
Defer the decision. She keeps the money in her account until she’s decided to keep the item (N-01). Evidenced.
Open each app separately before payday to see what’s due: Klarna, PayPal, and Riverty pay-later orders if she has any. Inferred from the hook and N-02.
Add the totals by hand to work out what will leave her account and when. From your hook.
Reconcile dates. Statement and due dates differ, and two reminders can arrive in one week for different amounts (T-104), so she has to work out which is real (T-103). Evidenced for Riverty’s own products.
Fall back to the bank card when she wants certainty: she taps it “without thinking” in shops (N-03), and test participants returned to debit after a failure (N-06). Evidenced.
- **Core frustration, the exact moment the process feels most “broken”:** Why it’s inefficient

No single source of truth. Each provider shows only its own balance, so the total exists only in her head. Participants already ask “which total is the real one” (T-103).
It scales with usage. Heavy users make 5.82 purchases per active month and put 25.4% on instalments, so they have the most items and dates to track. (These are card-level figures, not her total across providers.)
It falls on payday. The effort lands just when she has no cushion, so a miscount costs her.
Mistakes are expensive. Mismatched reminders (T-104) and late notifications (T-108) make people unsure whether a payment went through.
Adding Riverty makes it worse. N-02 says it plainly: a third app is one more thing to check.
- **The evidence, a specific quote or behavior from the research that proves this:** 155 approved users never activate and 143 cards never reach the wallet.
- **Your journey map file name (e.g. journey-map.html):** The timeline above shows the four stages. The details follow, each bullet in Action -> Benefit format.

1. **Stage name: Get approved**
   - **User action:** Uploads ID once and activates the card -> no repeat photo requests.
   - **Internal state:** Feels the process is quick -> she finishes instead of abandoning.
   - **Pain point addressed:** Re-upload loop (T-106) and 155 non-activations -> fewer approved users lost.

2. **Stage name: Add to wallet**
   - **User action:** Taps "add to wallet" on the approval screen -> card ready on her phone.
   - **Internal state:** Sees the card beside her bank card -> it becomes a real option.
   - **Pain point addressed:** 143 cards never reached the wallet (T-102) -> in-store payment becomes possible.

3. **Stage name: Pay, know why**
   - **User action:** Pays online or taps in store; any decline shows a reason -> no guessing.
   - **Internal state:** Feels informed even when a payment fails -> she retries instead of switching to debit.
   - **Pain point addressed:** Silent declines (T-101) and late push alerts (T-108) -> no double-paying, fewer fallbacks.

4. **Stage name: See one total**
   - **User action:** Opens one balance view before payday -> knows what leaves her account.
   - **Internal state:** Feels in control of Riverty amounts -> fewer manual sums and missed dates.
   - **Pain point addressed:** Separate screens and clashing dates (T-103, T-104) -> one total, one due date.

**Two limits to keep in mind**
- **The strategy overreaches.** "Switch from Klarna and PayPal" is not what these stages deliver. Stage 4 consolidates only Riverty's card and pay-later orders (B3, B8). Lena would still tally Klarna and PayPal by hand, so treat switching as an outcome to test, not a promise.
- **The scope may not fit an MVP.** The T-106 fix isn't in the B1-B8 backlog. B8 changes due dates, so under N-11 it may need months of approval. B3 alone could ship first, with Stage 4 showing one total before one due date.

**Three competitive advantages over the manual workaround**
1. Card and pay-later orders total automatically -> replaces adding Riverty amounts by hand.
2. One due date replaces mismatched reminders -> no payday surprises.
3. Declines explain themselves and offer a retry -> she stays on Riverty instead of falling back to debit.

These advantages hold against her manual tracking only. I haven't checked them against Klarna's or PayPal's own features, so verify before putting them in front of stakeholders.
- **Journey map:** _(not filled)_

### Slide 7 · Blueprint
- **Roadmap:** # Feature Roadmap, Module 4 · BU Pay & Credit

**Scenario:** Riverty BU Pay & Credit, First Consumer Card

**Team:** [your assumed team size]

## Strategic anchors
- **Persona:** Persona (M2):  The cautious occasional pay-later user. A light BNPL user who was approved for the card but never switched it on. They want to avoid interest and debt they didn’t plan for, and they get nervous when a product looks like credit or mentions instalments.
- **Primary metric:** Primary success metric (M3):  Approved → activated rate for light BNPL users. Baseline 62.0% (98 of 158 approved). Target 70% or more, stretch 74.7% (the regular-user rate).
- **Moment of misery:** Moment of misery (M2):  Approved, but unsure what the card costs or whether it hurts their credit score, the cautious occasional pay-later user hesitates at the activation screen and never switches the card on.
- **Guardrail:** Guardrail metric (M3):  Approved → activated rate for regular and heavy BNPL users (the healthy core). Baseline 77.8% combined (333 of 428 approved): 74.7% for regular, 82.6% for heavy. Floor of about 74%.

## Scoring
| Feature | Value | Effort | Quadrant | Decision | Rationale |
| B1 Decline reason and retry hint shown in the app | 1 | 1 | Fill-In | Later |  |
| B2 Add to phone wallet straight from the approval screen | 4 | 2 | Quick Win | Now |  |
| B3 One balance view for card and regular pay later orders | 5 | 3 | Major Project | Next |  |
| B4 Choose pay now or pay later per purchase after paying |  |  | · |  |  |
| B5 Offers from partner merchants inside the card app |  |  | · |  |  |
| B6 Cashback on every purchase |  |  | · |  |  |
| B7 |  |  | · |  |  |
| B8 |  |  | · |  |  |

### NOW, this sprint
- **B2 Add to phone wallet straight from the approval screen**, _rationale_

### NEXT, the following sprints
- **B3 One balance view for card and regular pay later orders**, _rationale_

### LATER, backlog
- **B1 Decline reason and retry hint shown in the app**, _rationale_

### ✂ Cut List
- _(none)_
- **PRD highlights:** # Add to phone wallet straight from the approval screen, Simplified PRD (Riverty BU Pay & Credit, First Consumer Card)

**Scenario:** Riverty BU Pay & Credit, First Consumer Card

**Author:** Me · **Status:** Draft · **Target:** High-Fidelity Prototype · **Persona:** The cautious occasional pay-later user. A light BNPL user who was approved for the card but never switched it on. They want to avoid interest and debt they didn’t plan for, and they get nervous when a product looks like credit or mentions instalments.

## 1. The Big Picture
- **Vision:** Every approved light pay-later user sees what the card costs and puts it in their phone wallet in one calm step, so approval turns into use.
- **Press release:** BU Pay & Credit makes switching on the new card a one-screen decision.

Right after approval, a short note says what the card costs, what it does not do, and whether it affects your credit score. One button then adds the card to your phone wallet. If you’re not ready, tap “Not now” and nothing is lost, because online purchases don’t need the wallet.

The change comes from people who were approved and still hesitated. One light pay-later user in the test launch said a credit card with interest is exactly what she tries to avoid, and that the word “instalments” makes her nervous. Others asked whether the card affects their credit score and found no answer. When a wallet add failed, nothing said why, and one participant went back to her debit card that week. Now the answer comes before the button, and a failed add says what happened and offers a retry.
- **Success metric:** Approved → activated rate for light BNPL users. Baseline 62.0% (98 of 158 approved). Target 70% or more, stretch 74.7% (the regular-user rate).
- **Guardrail:** Approved → activated rate for light BNPL users. Baseline 62.0% (98 of 158 approved). Target 70% or more, stretch 74.7% (the regular-user rate).

### User stories
- User stories (one per line):
- As a cautious light pay-later user who has just been approved, I want to read in plain words what the card costs and whether it affects my credit score, so that I can switch it on without fearing interest or debt I did not plan for.
- As an approved user who wants to pay in shops, I want to add the card to my phone wallet with one tap from the approval screen, so that I do not have to remember another card at the till.
- As an approved user who is not ready, or whose wallet add fails, I want a plain reason and a choice to retry or skip, so that I never feel pushed or stuck.
### Screens to build
- Screens to build (exactly 3, at 360 px width):
- Screen 1: Entry point, the approval screen
- Heading: “You’re approved”.
- Card image with a masked fictional number (•••• 4821) and a fictional name.
- Cost note, two to three lines, answering what the card costs, what it does not do, and whether it affects the credit score. The prototype shows placeholder copy with a visible “placeholder, not approved” label.
- Primary button, full width, at least 48 px tall: “Add to wallet”.
- Secondary text button below it: “Not now”.
- Screen 2: Feature core, adding to the wallet (two states)
- Progress state: card thumbnail, spinner, status line “Adding your card to your wallet”. No buttons, and taps are ignored while it runs.
- Failure state: heading “We couldn’t add your card”, one reason line, primary button “Try again”, secondary button “Not now”.
- Fixed reasons: (1) connection lost, (2) wallet not available on this phone, (3) took longer than 5 seconds. Reason 2 hides “Try again” and the second button reads “Continue”, since a retry cannot help.
- Screen 3: Success and confirmation (two variants)
- Added: check mark, heading “Your card is in your wallet”, card image with an “In wallet” tag, one line “Use it online or at the till”, button “Done”.
- Skipped or gave up: heading “Your card is ready”, one line “You can use it online now. Adding it to your wallet is only needed to pay in shops”, button “Done”.
- What each screen rests on
- Screen 1: the cost note answers N-05 and T-107. It is the only part of the prototype that touches the activation hesitation behind your primary metric (62.0% baseline).
- Screen 2: the fixed reasons and the “Try again” or “Not now” choice answer N-06 and T-102, where a silent failure sent a participant back to her debit card.
- Screen 3: the skipped variant relies on the pack’s note that online purchases don’t need the wallet. Neither variant shows rewards, offers or instalment wording, because N-05 says instalments make this persona nervous.
- Check before you build
- The cost note is a placeholder. The pack has no figures on cost or credit-score impact, so the final wording has to come from compliance.
- Screens 2 and 3 have two states each. That keeps the count at three, but the prototype needs both states built and reachable.
- Open question for engineering: whether confirming on this screen counts as activation. The skipped variant assumes it does (“Your card is ready”), so that wording changes if activation happens elsewhere.
- The 5-second timeout and 48 px button height are my suggestions, not from the pack.
- I can write the functional requirements next.
### Functional requirements
- Functional requirements (8, from the Must-Haves M1 to M5):
- ID	Requirement	Source
- FR1	Screen 1 shows the “Add to wallet” button inside the first 640 px of height at 360 px width, with no scrolling.	M1
- FR2	The cost note is 40 words or fewer, sits directly above the button, and answers cost, what the card does not do, and credit-score effect. Only compliance-approved text ships.	M3
- FR3	One tap on “Add to wallet” shows the progress state in 300 ms or less. Taps during progress are ignored, so the card cannot be added twice.	M1
- FR4	Every add attempt ends in success or failure within 5 seconds. None ends silently or spins longer.	M2
- FR5	Every failure shows one of three fixed reasons, plus “Try again” and “Not now”. “Try again” is hidden when the wallet is unavailable (the second button then reads “Continue”), and is allowed at most 3 times per session.	M2
- FR6	“Not now” is one tap on Screen 1 and on the failure state. It leads to the skipped variant of Screen 3, never blocks the card, and the prompt does not return in the same session.	M4
- FR7	Screen 3 shows the “in your wallet” variant only after a confirmed success. No screen shows rewards, offers or instalment wording.	M2
- FR8	Six events are logged with a timestamp and a segment tag (light, regular, heavy): screen viewed, add started, add succeeded, add failed (with reason), add retried, skipped.
### Smart behaviors (Situation → Outcome)
- Smart behaviors (Situation → Outcome, one per line):
- If any approved user reaches Screen 1, then show the same screen and the same cost note to every segment. The segment is recorded in events only.
- If the user taps “Add to wallet” and it succeeds within 5 seconds, then show Screen 3, “in your wallet” variant, and log add succeeded.
- If the add fails because the connection dropped, then show the Screen 2 failure state with reason 1, “Try again” and “Not now”.
- If the wallet is not available on this phone, then show the failure state with reason 2, hide “Try again”, and make the one button “Continue”, which leads to the skipped variant.
- If there is no result after 5 seconds, then show the failure state with reason 3, “Try again” and “Not now”.
- If the third retry in one session fails, then remove “Try again” and keep only “Not now”.
- If the user closes the wallet sheet or taps back during progress, then return to Screen 1 with no error message, and log add failed with reason “cancelled by user”.
- If the user taps “Add to wallet” twice quickly, then ignore the second tap and log one attempt.
- If the user taps “Not now” on Screen 1, then show Screen 3, skipped variant, log skipped, and do not prompt again this session.
### Technical constraints
- Technical constraints: what not to build
- No external APIs. No real wallet provisioning, card issuing or analytics service. Wallet outcomes are simulated with timers.
- No database and no backend. Nothing is sent to or stored on a server.
- No login or accounts. The prototype opens straight onto Screen 1.
- No saved data. State lives in memory, and a reload restarts the flow.
- One HTML file with plain JavaScript and CSS. No frameworks, no CDN scripts, no image files. The card is drawn with CSS.
- No real personal or card data. A fictional name and a masked number only (•••• 4821).
- No final legal copy. The cost note is labelled “placeholder, not approved” until compliance signs it off.
- No extra screens. One prototype-only control strip outside the phone frame forces an outcome (success, connection lost, wallet unavailable, slow) and shows a read-only event log. It is not a fourth screen and is not part of the product.
- Fixed 360 px phone frame. No desktop layout beyond centring it.

## MoSCoW scope
- **Must:** MUST HAVE (sprint 1); #	Requirement	Why it passes the test; M1	An “Add to wallet” action on the approval screen, shown the moment approval is confirmed	It is the feature itself. Without it nothing ships.; M2	A clear success state, and a failure state that says what went wrong and offers a retry	T-102 shows adds that fail or get abandoned, and N-06 shows what silent failure does: she went back to her debit card that week.; M3	One plain-language line above the button on what the card costs and what it does not do, including the credit-score answer	This is the only must-have that addresses the hesitation. The wording needs compliance sign-off, and it must not change pricing or terms (N-11).; M4	A “Not now” option that never blocks activation	Online purchases don’t need the wallet, so forcing the step would add friction for people who don’t need it. It also protects your guardrail on regular and heavy users (74% floor).; M5	Events for step viewed, wallet-add started, succeeded, failed and skipped, split by BNPL segment	This is not user-facing, so it fails your ruthless test, but I’m keeping it. Without it you can’t read the 66.8% baseline or the light-user split at the decision point.; If you won’t ship M3 (for example because compliance is slow), then no must-have on this list addresses the moment of misery. In that case say that B2 is a wallet-completion fix, not an activation fix.
- **Should:** SHOULD HAVE (if capacity allows); A way back to the wallet step later from the card screen, for people who tapped “Not now”. N-03 says people forget the card exists.; Hide the wallet step on devices that can’t use it, so those users don’t hit a dead end.; A quick copy check of M3 with 3 to 5 light users before release.
- **Could:** COULD HAVE (V2); A reminder nudge if the card isn’t in the wallet after a set number of days. T-108 shows late push messages cause confusion, so fix timing first.; Offer to set the card as the default payment method in the wallet.; Prompt to add the card after the first online purchase, for people who skipped it.; Copy that varies by user segment.; A balance or limit view from the wallet entry (this overlaps with B3).
- **Won't (now):** WON’T HAVE (NOW); Decline reasons or retry hints for in-store payments (B1). T-101 is a separate fix.; A combined balance view or one due date (B3, B8).; Any reward for adding to the wallet, such as cashback or partner offers (B5, B6). N-12 says incentives drive a trial, not keeping the card.; Any change to pricing, credit policy, terms or instalment options (B4). N-11 says this takes months.; Changes to the identity check or approval logic (T-106).; A full credit-score help centre article. M3 is one line only, and the article is separate work.; Physical card (B7).
- **Prototype:** https://github.com/costir777/product-management-template/blob/main/04-roadmap/prototype.html.html

### Slide 8 · Validation
## Parameters
| Parameter | Decision |
| Feature under test | B2	Add to phone wallet straight from the approval screen |
| Persona | Riverty_persona |
| Expected outcome | Increase the rate of activated cards |
| Primary success metric | Number of activated cards out of total cards |
| Baseline rate | 66.8 |
| Guardrail metric | 65 |
| Guardrail boundary | · |
| Second guardrail | · |
| Minimum Detectable Effect | +5p |
| Sample size per arm | 4,144 |
| Traffic split | 50/50 |
| Test duration | 21days |
| Significance threshold | 95% |

## Control vs. Variant
- **Control (A):** Activated to added to phone wallet is only 66%, while shall be 80%+
- **Variant (B):** CTA: Add your card now to wallet as a big large button on the screen and get 3 EUR bonus to spend
- **Held constant (isolation check):** App version

### Slide 9 · Launch
- **GTM:** ## Get your prior work ready
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
- **Metrics:** _(not filled)_

### Slide 10 · Story
- **Friction + aha:** Lots of steps in the journey :)
- **Takeaways / next:** How a clear step by step structure can optimize the time to market for a new product

---

Submitted to the Product Management Certification learning platform · Product School.
