Minimum Viable Attributes (MVA)

## Definition

MVA are the set of MITS elements/attributes required to be transmitted within a charge offer item for a receiving system to properly display and use in a pricing calculator.

## MVA Attributes

### Charge Offer Class

- Code
- Assumptions if attributes are excluded:
  - Limits:
    - **Maximum Occurrences:** unless provided, assume no limit subject to receiving system policies.
    - **Maximum Amount:** unless provided, assume no limit, subject to receiving system policies.

### Charge Offer Item

- Internal Code
- Name
- Description (if relevant)
- Characteristics
  - Requirement
  - Lifecycle
  - Payment Frequency
- Amount Basis
- Amount Per Type
- Amount Per Period (if "Period" is selected as the Amount Per Type)
- Percentage Of Code (if Amount Basis is set to "Percentage Of")
- Refundability (if relevant)
- Assumptions if attributes are excluded:
  - **Refundability:** Non-refundable.
  - **Item Max Occurrences:** unless provided, assume no limit, subject to receiving system policies.

### Charge Offer Amount

- Amounts
- Percentage (if Amount Basis is set to "Percentage Of")
- Duration (required for rent charges offering differing amounts for different lease durations)
- Assumptions if attributes are excluded:
  - **Term Basis:** Whole Lease.
