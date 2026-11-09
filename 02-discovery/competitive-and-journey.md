# Competitive Analysis & Journey Map (Module 2)

## Responses
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
