# IFRS 9 and IFRS 7 Credit Loss Agent

Classification, effective interest, expected credit losses, POCI, modifications, hedge accounting and the matching IFRS 7 risk disclosures.

> FOR DEMONSTRATION AND EDUCATIONAL PURPOSES ONLY. This output is not accounting, audit, tax or legal advice, and no liability whatsoever is assumed for its results or for any decision based on them. Paragraph references point to the IFRS Accounting Standards issued by the IASB; the standards' text is not reproduced. Results depend entirely on the facts entered and must be independently verified by a qualified professional against the current authoritative text before any use.

**Standards:** IFRS 9 Financial Instruments; IFRS 7 Financial Instruments: Disclosures
**Tools:** 18 calculators, checklists and lookups, plus `agent_about`
**For:** Bank and lender finance teams, credit risk analysts, treasury and financial-instruments auditors.

## What it does

- Classify assets with the business model and SPPI tests
- Build effective interest schedules, including credit-adjusted EIR for POCI
- Compute 12-month and lifetime ECL and provision matrices
- Account for modifications, derecognition, own credit and hedges
- Prepare loss-allowance reconciliations, maturity analysis and sensitivity disclosures

Every result cites the IFRS paragraphs it relies on. The standards' text is paraphrased, never reproduced.

## Install

With the mcprush CLI (after buying the listing):

```bash
npx mcprush add <publisher>/ifrs9-credit-loss-agent
```

Or point any MCP client at the bundled server (Node.js 22+, no dependencies, no network, no API keys):

```json
{ "mcpServers": { "ifrs9-credit-loss-agent": { "command": "node", "args": ["<path>/ifrs9-credit-loss-agent/dist/server.mjs"] } } }
```


## Try it

> A loan book of 10m in stage 1 has PD 2%, LGD 45%; 1m in stage 2 has lifetime PD 15%. Compute the ECL and the IFRS 7 loss allowance reconciliation.

## Tools

| Tool | What it does |
|---|---|
| `ifrs9_classification` | Classification of financial instruments |
| `ifrs9_effective_interest_schedule` | Effective interest rate & amortised cost |
| `ifrs9_expected_credit_loss` | ECL staging & measurement |
| `ifrs9_modification` | Modification & the 10% test |
| `ifrs9_derecognition` | Derecognition of financial assets |
| `ifrs9_hedge_accounting` | Hedge effectiveness & accounting |
| `ifrs9_lookup` | Paragraph & topic lookup |
| `ifrs9_own_credit` | Own credit risk on liabilities designated at FVTPL (5.7.7) |
| `ifrs9_poci` | Purchased or originated credit-impaired assets: credit-adjusted EIR (5.4.1(a), 5.5.13) |
| `ifrs7_disclosure_checklist` | Disclosure checklist |
| `ifrs7_categories_and_fair_value` | Categories & fair value comparison (8, 25-29) |
| `ifrs7_loss_allowance_reconciliation` | Loss allowance reconciliation (35H) |
| `ifrs7_provision_matrix` | Provision matrix for trade receivables (35N) |
| `ifrs7_liquidity_maturity_analysis` | Liquidity maturity analysis (39, B11) |
| `ifrs7_market_risk_sensitivity` | Market risk sensitivity (40) |
| `ifrs7_offsetting` | Offsetting & master netting (13A-13F) |
| `ifrs7_lookup` | Paragraph & topic lookup |
| `ifrs7_supplier_finance` | Supplier finance arrangements (IAS 7.44F-44H, B11F(j)) |

## Sample output (`ifrs9_classification`, built-in example)

Sustainability-linked corporate loan: Amortised cost.

## Privacy and safety

- Runs locally over stdio. No network calls, no telemetry, no files written.
- Every tool is read-only, idempotent and closed-world (MCP annotations declared).
- No personal data is collected.

Demo and educational use only. No liability assumed for results. Not professional advice.
