# PRD & Prototype Sprint (Module 4)

## Pick & scope with MoSCoW
- **The “Now” feature I’m scoping (name + one-line core description):** Add to phone wallet straight from the approval screen
- **My finalized Must-Haves (after overriding the AI):** MUST HAVE (sprint 1)

#	Requirement	Why it passes the test
M1	An “Add to wallet” action on the approval screen, shown the moment approval is confirmed	It is the feature itself. Without it nothing ships.
M2	A clear success state, and a failure state that says what went wrong and offers a retry	T-102 shows adds that fail or get abandoned, and N-06 shows what silent failure does: she went back to her debit card that week.
M3	One plain-language line above the button on what the card costs and what it does not do, including the credit-score answer	This is the only must-have that addresses the hesitation. The wording needs compliance sign-off, and it must not change pricing or terms (N-11).
M4	A “Not now” option that never blocks activation	Online purchases don’t need the wallet, so forcing the step would add friction for people who don’t need it. It also protects your guardrail on regular and heavy users (74% floor).
M5	Events for step viewed, wallet-add started, succeeded, failed and skipped, split by BNPL segment	This is not user-facing, so it fails your ruthless test, but I’m keeping it. Without it you can’t read the 66.8% baseline or the light-user split at the decision point.

If you won’t ship M3 (for example because compliance is slow), then no must-have on this list addresses the moment of misery. In that case say that B2 is a wallet-completion fix, not an activation fix.
- **What I demoted from Must → Should/Won’t, and why:** Copy that varies by user segment as it's not critical for now

## Generate your Simplified PRD
- **One thing my PRD makes explicit that a vague brief would have missed:** Structure clarity

## Prompt-to-prototype sprint
- **Where did the prototype reveal a gap in my PRD logic? (what I had to update):** These are gaps I hit while writing the code. I haven’t run the file in a browser, so none of them came from testing.

Reason 2 contradicts Story 3. Story 3 says “Not now” appears on the failure state of Screen 2. FR5 says that for “wallet not available” the second button reads “Continue” and there is no retry. I followed FR5. I also logged that tap as skipped, though the user didn’t choose to skip. The PRD should say whether “Continue” counts as skipped or needs its own event.
“Already in wallet” contradicts FR7. The edge case sends the user straight to the “in your wallet” variant with no add. FR7 allows that variant only after a confirmed success. I followed the edge case and logged no add succeeded. FR7 needs an exception, and the log needs a way to mark “pre-existing”.
A retry during a late success could add the card twice. You say not to offer a retry once a late success arrives, and the card can’t be added twice. But nothing says what happens if the user taps “Try again” at 5.1 s and the first add then succeeds at 6 s. In my build a new attempt cancels the old one, so the UI ignores a card that really was added. The PRD should require a wallet-state check before any retry.
Cancel during progress has no trigger. Progress has “no buttons” and ignores taps, yet “user closes the wallet sheet or taps back” must return to Screen 1. Nothing in the three screens lets the user do that, so I put a “Cancel during progress” button in the control strip. Logging it as add failed with the reason “cancelled by user” also gives a fourth reason, although FR5 says failures use three fixed ones.
Done has no defined destination. The PRD never says where “Done” goes, and that ties to your open question about activation. I made it restart the flow as a new session. That also means “no repeat prompt this session” depends on a session definition the PRD doesn’t give.
The comprehension eval can’t be run on this prototype. The cost note is a labelled placeholder, so testers have no real answers to restate. The 4-of-5 test only works once compliance text exists. The PRD should say whether the test waits for that text or uses a clearly marked stand-in.
The retry cap is ambiguous. FR5 says “at most 3 times”. The smart behaviours say “third failed retry”. I hid “Try again” after the third retry has failed, which allows four attempts in total. The PRD should say whether the cap counts retries or attempts.

For the PRD update, items 1 to 3 change behaviour and need decisions. Items 4 to 7 are mostly wording.
- **My prototype: save Claude's HTML as prototype.html in 04-roadmap/, open it in your browser, and add a screenshot:** _(not filled in)_
