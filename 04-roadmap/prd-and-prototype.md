# Add to phone wallet straight from the approval screen, Simplified PRD (Riverty BU Pay & Credit, First Consumer Card)

**Scenario:** Riverty BU Pay & Credit, First Consumer Card

**Author:** Me · **Status:** Draft · **Target:** High-Fidelity Prototype · **Persona:** The cautious occasional pay-later user. A light BNPL user who was approved for the card but never switched it on. They want to avoid interest and debt they didn’t plan for, and they get nervous when a product looks like credit or mentions instalments.

## 1. The Big Picture
- **Vision:** Every approved light pay-later user sees what the card costs and puts it in their phone wallet in one calm step, so approval turns into use.
- **Press release:** BU Pay & Credit makes switching on the new card a one-screen decision.

Right after approval, a short note says what the card costs, what it does not do, and whether it affects your credit score. One button then adds the card to your phone wallet. If you’re not ready, tap “Not now” and nothing is lost, because online purchases don’t need the wallet.

The change comes from people who were approved and still hesitated. One light pay-later user in the test launch said a credit card with interest is exactly what she tries to avoid, and that the word “instalments” makes her nervous. Others asked whether the card affects their credit score and found no answer. When a wallet add failed, nothing said why, and one participant went back to her debit card that week. Now the answer comes before the button, and a failed add says what happened and offers a retry.
- **Success metric:** Approved → activated rate for light BNPL users. Baseline 62.0% (98 of 158 approved). Target 70% or more, stretch 74.7% (the regular-user rate).
- **Guardrail:** Approved → activated rate for light BNPL users. Baseline 62.0% (98 of 158 approved). Target 70% or more, stretch 74.7% (the regular-user rate).

## 2. The Details
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

## 3. The Logistics
### Features out
_exclusions_
### Edge cases & safety guard
_unhappy paths_
### Decision log
_scope choices_
### Evals
_success targets_

## MoSCoW scope
- **Must:** MUST HAVE (sprint 1); #	Requirement	Why it passes the test; M1	An “Add to wallet” action on the approval screen, shown the moment approval is confirmed	It is the feature itself. Without it nothing ships.; M2	A clear success state, and a failure state that says what went wrong and offers a retry	T-102 shows adds that fail or get abandoned, and N-06 shows what silent failure does: she went back to her debit card that week.; M3	One plain-language line above the button on what the card costs and what it does not do, including the credit-score answer	This is the only must-have that addresses the hesitation. The wording needs compliance sign-off, and it must not change pricing or terms (N-11).; M4	A “Not now” option that never blocks activation	Online purchases don’t need the wallet, so forcing the step would add friction for people who don’t need it. It also protects your guardrail on regular and heavy users (74% floor).; M5	Events for step viewed, wallet-add started, succeeded, failed and skipped, split by BNPL segment	This is not user-facing, so it fails your ruthless test, but I’m keeping it. Without it you can’t read the 66.8% baseline or the light-user split at the decision point.; If you won’t ship M3 (for example because compliance is slow), then no must-have on this list addresses the moment of misery. In that case say that B2 is a wallet-completion fix, not an activation fix.
- **Should:** SHOULD HAVE (if capacity allows); A way back to the wallet step later from the card screen, for people who tapped “Not now”. N-03 says people forget the card exists.; Hide the wallet step on devices that can’t use it, so those users don’t hit a dead end.; A quick copy check of M3 with 3 to 5 light users before release.
- **Could:** COULD HAVE (V2); A reminder nudge if the card isn’t in the wallet after a set number of days. T-108 shows late push messages cause confusion, so fix timing first.; Offer to set the card as the default payment method in the wallet.; Prompt to add the card after the first online purchase, for people who skipped it.; Copy that varies by user segment.; A balance or limit view from the wallet entry (this overlaps with B3).
- **Won't (now):** WON’T HAVE (NOW); Decline reasons or retry hints for in-store payments (B1). T-101 is a separate fix.; A combined balance view or one due date (B3, B8).; Any reward for adding to the wallet, such as cashback or partner offers (B5, B6). N-12 says incentives drive a trial, not keeping the card.; Any change to pricing, credit policy, terms or instalment options (B4). N-11 says this takes months.; Changes to the identity check or approval logic (T-106).; A full credit-score help centre article. M3 is one line only, and the article is separate work.; Physical card (B7).

