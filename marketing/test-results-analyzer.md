# Test Results Analyzer

## Outcome
Determine experiment winners with statistical confidence and explain why they won.

## Inputs
- Experiment data (from experiment-tracker)
- Raw metrics per variant (conversions, engagement, revenue)
- Sample sizes and duration
- Success criteria defined at experiment start

## Steps
1. Pull experiment data and verify sufficient sample size
2. Calculate metrics per variant
3. Run statistical significance test (p-value, confidence interval)
4. Determine winner, loser, or inconclusive
5. Calculate lift (% improvement of winner vs control)
6. Analyze secondary metrics (did winner hurt anything else?)
7. Hypothesize WHY the winner won (creative, timing, audience)
8. Recommend next action: scale winner, iterate, or new test

## Outputs
- Results report: winner, lift %, confidence level
- Statistical analysis summary
- Secondary metrics impact
- Hypothesis for why winner won
- Recommended next action

## Boundaries
- ✅ Analyzes experiment results
- ✅ Determines statistical significance
- ✅ Explains why variants won/lost
- ✅ Recommends next actions
- ❌ Does NOT track experiments (owned by experiment-tracker)
- ❌ Does NOT design experiments (owned by relevant team)
- ❌ Does NOT implement winning variants (owned by engineering/marketing)
- ❌ Does NOT make final scaling decisions (owned by product-manager)
