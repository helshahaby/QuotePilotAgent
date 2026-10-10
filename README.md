# QuotePilot

**Arabic / English sales quotation agent for small suppliers**  
**Author:** Hossam Elshahaby  
**Hackathon:** Agents at Work 2026

- [Live application](https://quotepilotagent.lovable.app)
- [Demo video](https://youtu.be/nVatsv9ev48)

## Project overview

QuotePilot helps small electrical and automotive parts suppliers prepare quotations from Arabic and English customer inquiries. The agent interprets the request, searches catalog and inventory data, and uses code to calculate pricing. The owner reviews the quotation before finalization or customer sending.

## Problem and target users

Small supplier owners and sales staff repeatedly search product catalogs, check stock, and calculate quotations while handling customer messages. Incomplete specifications and mixed-language requests add clarification work. QuotePilot targets this inquiry-to-quotation workflow so owners can spend less time on repetitive administration and more time serving customers.

## Product capabilities

The public application describes these capabilities:

- Arabic and English inquiry understanding.
- Extraction of requested items and identification of missing information.
- Product matching against catalog data and inventory lookup.
- Deterministic price, discount, and VAT calculations.
- Quotation draft creation and an activity log of agent tool use.
- Owner approval before quotation finalization or customer sending.

## How the agent works

1. The user submits a customer inquiry.
2. The agent extracts items, quantities, and specifications.
3. Catalog-search and inventory tools retrieve business records.
4. Missing or ambiguous information requires clarification.
5. Code calculates the quotation using the configured pricing rules.
6. The agent saves a draft for the owner to review and approve.

The public activity-log example lists `record_extraction`, `search_catalog`, `lookup_inventory`, `calculate_quote`, and `save_quote_draft`. A language model interprets the request, while business tools supply catalog records and calculate totals. The exact model provider and backend framework are not documented here because source code was not provided.

## Try the hosted application

1. Open [QuotePilot](https://quotepilotagent.lovable.app).
2. Choose **Open workspace** and sign in using your own account or access supplied by the project owner.
3. Use catalog and inventory data available in that account.
4. Enter an inquiry for a product in the catalog, for example: `Please quote 10 units of MCB 1P 16A and confirm stock.`
5. Review product matches, stock availability, tool activity, and quotation totals.
6. Check the draft and approval step. Identify sample data clearly during demonstrations.

Watch the [demo video](https://youtu.be/nVatsv9ev48) for the recorded walkthrough. This README provides hosted testing instructions. Local installation commands and environment variables must come from the actual source repository.

## Business impact and evaluation

The intended benefit is less manual searching and more consistent quotation preparation. No measured time savings, cost savings, or revenue results were provided for these materials.

Evaluate the same 10 inquiries manually and with QuotePilot using the same catalog. Include exact matches, incomplete requests, ambiguous specifications, and unavailable stock. Record manual time, agent processing time, owner review time, corrections, and calculation errors.

- **Time saved:** manual processing time minus agent processing time minus owner review time.
- **Net labor cost saved:** saved hours multiplied by the SME hourly labor cost, minus incremental operating costs.
- **Quality:** correct product matches, correct totals, and the number of corrections per quotation.
- **Revenue:** record actual won orders separately. Order value alone does not establish that the agent generated additional revenue.

Keep measured results separate from projections and sample data.

## Reliability and approval

Catalog and inventory records should remain the source of product specifications, prices, and stock. The public app states that it does not invent these values and that it requires approval before anything is finalized or sent. Human review remains necessary for uncertain product matches and business decisions.

## Current status and limitations

- A public hosted app is available at the link above.
- Feature descriptions reflect the public app copy. The authenticated workflow and backend were not independently audited for this documentation.
- No named SME pilot, benchmark export, or measured business results were supplied.
- The demo link was provided by the project owner. The video contents were not independently reviewed for this documentation.
- Catalog freshness and account configuration affect quotation quality.

## Next steps

Run a measured pilot with one supplier, validate ambiguous and out-of-stock requests, and publish benchmark evidence including human review time. Possible future extensions include follow-up reminders and confirmed integrations with business systems.

## Submission materials

- Public GitHub repository with the actual working source and setup instructions.
- Impact slides describing the SME, replaced workflow, and measured results.
- A 2-3 minute demonstration video.
- Project description PDF and this README.

## Author

Hossam Elshahaby - electrical and software engineer with more than 10 years of embedded and automotive engineering experience.
