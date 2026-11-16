# A/B Experiment Brief, Riverty BU Pay & Credit, First Consumer Card

## Parameters
| Parameter | Decision |
|---|---|
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

## Hypothesis
> I believe that B2	Add to phone wallet straight from the approval screen for Riverty_persona will result in Increase the rate of activated cards, as measured by a +5p change in Number of activated cards out of total cards within 21days. We will protect 65 throughout the test.

## Shipping criteria
> We will **ship** if Number of activated cards out of total cards improves by ≥ +5p at 95% and 65 does not reach _(not filled in)_ after 21days.
> We will **iterate** if direction is positive but lift is below the MDE.
> We will **kill** if the primary metric shows no improvement or moves negatively.
> The read date is fixed at the end of 21days, no results reviewed before this date.
