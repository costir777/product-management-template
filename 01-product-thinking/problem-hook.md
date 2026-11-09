# Problem Hook & Value Proposition (Module 1)

## Responses
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
