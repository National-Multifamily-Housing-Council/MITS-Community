# Total Monthly Leasing Price (TMLP)

## Definition

TMLP is the amount displayed to the consumer as their expected recurring monthly price/cost.

## TMLP Components

In general terms:

Base Rent w/ all lease term duration options transmitted (if no lease term duration options transmitted, assume 12 month term) + Monthly Mandatory Fees.

### Excluded

- optional fees
- mandatory fees not charged monthly
- variable fees without explicit values

Specifically, any charge offer item where the following MVA elements are set:

### "Advertisement/Search" Context

When calculating TMLP in an "Advertisement/Search" context:

- Requirement = "Mandatory"
- Lifecycle = "During Term"
- Payment Frequency = "Monthly"
- Amount per Type = "Item"

### "Detailed Calculator" Context

When calculating TMLP in a "Detailed Calculator" context:

- "Advertisement/Search" charge items PLUS any selected monthly "Optional" and corresponding "Conditional" charges

### Assumptions

- Transmitted files must use cents for price/cost data; do not round amounts in the transmitted data.
- Exclude charge items set to "Estimate" and "Variable" but display as "Tooltips" for information so consumer is aware of potential additional cost.
- Ranges for fees other than BASE RENT:
  - If limited display space, display upper bound calculated amounts.
  - If display space allows, display both lower and upper bound range calculations.
- For BASE RENT charges covering a range of values within a list of available units, the lowest cost value may be displayed.