# AI Synthesis, Product Health & Insights Summary (Module 2)

## Responses
- **Assumption to validate #1:** A new card from Riverty will become top of mind for many of our users
- **Assumption to validate #2:** The users will find it easy to pay in stores or online
- **Assumption to validate #3:** There will be less than 0.1% declined transactions
- **Moment of misery / red flag #1 (e.g., “user gave up after 3 tries”):** Failing identity check
- **Moment of misery / red flag #2:** Failing to show same data for card balance on different screens
- **Moment of misery / red flag #3:** Faillng to show same due dates on various screens
- **Product Health & Insights Summary (Claude's output):** # Product Health & Insights Summary

**Scope:** 12 interview notes (N-01 to N-12) and 8 bug/ticket reports (T-101 to T-108). All data is illustrative and fictional.

## Executive Summary

The card's core payment rails function, but they fail often enough in visible, unexplained ways to damage trust during the moments that matter most (in-store payment and wallet activation). Users who like the underlying "pay later" behaviour are confused by how the card is presented, how it relates to existing products, and what it costs them. The most important caveat is that the test group is skewed toward colleagues, so current approval and repayment signals probably overstate real-world performance.

## Thematic Synthesis

### 1. Technical Stability & Payment Reliability

Payment failures cluster around two points: the in-store transaction and the move from card activation to phone wallet. In both cases the failure is silent or unexplained, which turns a technical fault into a behavioural one. At least one participant abandoned the card for her debit card after a single decline. Delayed notifications compound this by prompting double payment.

- **In-store declines with no reason shown in the app (T-101, N-06):** 48 declines in the test log, with users defaulting back to their debit card. **Critical**
- **Wallet provisioning failure or abandonment after activation (T-102):** 143 activated cards never reached the wallet, which blocks the primary tap-to-pay use case. **Critical**
- **Late purchase push notifications (T-108):** Users assume payment failed and pay again with another card, creating duplicate spend. **High**

### 2. Onboarding & Activation Friction

Onboarding loses applicants at identity verification, and activation loses them again at the wallet step. Both drop-offs happen before the card has had any chance to prove its value.

- **Repeated document photo request after a failed upload (T-106):** Some applicants abandon at this step. **High**
- **Wallet setup abandonment (T-102):** Overlaps with stability but is also a funnel-conversion issue. **High**

### 3. Trust, Clarity & Mental Model

Users struggle to place the card relative to existing pay later products and to credit cards. The product presents financial information in fragmented ways, and users read ambiguity as risk. Language such as "instalments" triggers aversion among users who associate it with interest-bearing credit. The appeal of the underlying behaviour is real (deferring payment until after keeping the item), but the card does not yet make its own proposition legible.

- **Split balance across two screens (T-103, N-07):** Users cannot determine what they owe in total or which figure is authoritative. **High**
- **Misaligned statement and due dates, producing duplicate reminders for different amounts (T-104):** **High**
- **Unclear credit-score impact, with no help content (T-107):** **Medium**
- **Instalment option appears post-purchase for some categories only, perceived as random (T-105):** **Medium**
- **Perception of credit-card-like cost, with "instalments" language creating nervousness (N-05):** **Medium**
- **Card is easy to forget at point of sale versus default bank card (N-03):** **Medium**

### 4. Value Proposition & Adoption

Demand is conditional. Heavy BNPL users show strong latent interest, particularly for everyday and grocery spend, but they already juggle multiple similar apps, and incentives (e.g. cashback) may drive trial more than retention. Merchants are sceptical that the card gives them a reason to be chosen at checkout, and SME merchants are only interested if it drives traffic to them rather than to large marketplaces.

- **App fatigue and competition from existing BNPL apps (N-02):** **Medium**
- **Unproven retention beyond incentive-driven trial (N-12):** **Medium**
- **Merchant value unclear, especially for enterprise merchants (N-08, N-09):** **High**
- **Demonstrated demand for everyday and grocery use (N-04, N-01):** Positive signal; no severity assigned.

### 5. Data Validity & Delivery Constraints

Two internal observations qualify how far the above findings can be trusted and acted on.

- **Test cohort skews toward colleagues (N-10):** Approval and repayment metrics are likely to look better than real-customer performance. **High**
- **Proposition changes require lengthy approval for pricing, credit policy and terms (N-11):** Structural constraint on iteration speed, measured in months. **Medium**

### 6. Support Load

Several issues above are likely to generate inbound contact: unexplained declines, balance confusion, duplicate reminders and credit-score questions. The missing help article is a direct gap in self-service.

- **Absence of self-service content on credit-score impact and balance/due-date logic (T-107, T-103, T-104):** **Medium**

### Minor Technical Debt

Inconsistent post-purchase instalment eligibility messaging, notification timing variance outside affected shops, and minor copy and labelling inconsistencies across balance and statement screens.
- **Did the AI catch the specific moment of misery / pain point you found in Step 1?:** Yes
- **Did it smooth over a critical frustration into a generic bullet point?:** No
- **Did the AI try to suggest features or a roadmap despite the constraints?:** No
- **Logic leak / hallucination #1 (e.g., “AI suggested a new search bar feature, roadmap leak”):** _(not filled in)_
- **Logic leak / hallucination #2:** _(not filled in)_
