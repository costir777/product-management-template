# Hypothesis & Success Metrics (Module 3)

## Pre-work · Hypothesis check
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
