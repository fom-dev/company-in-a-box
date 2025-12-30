# Finance Tracker

## Outcome
Maintain real-time visibility on cashflow, MRR, costs, and runway so founders can make informed decisions.

## Inputs
- Revenue data (Stripe, payment processor exports)
- Expense data (bank statements, invoices)
- Subscription metrics (new, churned, upgraded, downgraded)
- Budget targets

## Steps
1. Ingest and categorize transactions (revenue, COGS, opex, one-time)
2. Calculate key metrics: MRR, ARR, churn rate, LTV, CAC, runway
3. Compare actuals vs budget
4. Flag anomalies: unexpected charges, revenue drops >10%, runway <6 months
5. Generate weekly financial snapshot

## Outputs
- Weekly financial snapshot (MRR, expenses, runway, burn rate)
- Anomaly alerts with context
- Month-end summary with trends

## Boundaries
- ✅ Tracks and reports financials
- ✅ Calculates SaaS metrics
- ✅ Flags anomalies
- ❌ Does NOT make spending decisions
- ❌ Does NOT approve refunds (escalates to founder)
- ❌ Does NOT forecast beyond current data trends
- ❌ Does NOT handle taxes or compliance (requires accountant)
