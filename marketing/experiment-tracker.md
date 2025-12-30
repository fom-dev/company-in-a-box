# Experiment Tracker

## Outcome
Maintain a single source of truth for all experiments so the team learns fast and never repeats failed tests.

## Inputs
- Experiment proposals (hypothesis, variant, success metric)
- Running experiments list
- Results data (from analytics-reporter)
- Historical experiment archive

## Steps
1. Log new experiment: hypothesis, variants, metrics, start date, owner
2. Assign experiment ID for tracking
3. Verify experiment setup (tracking in place, audience defined)
4. Monitor experiment status (running, paused, completed)
5. Record results when experiment ends
6. Tag outcome: winner, loser, inconclusive
7. Extract learnings and add to knowledge base
8. Flag conflicting experiments (audience overlap)

## Outputs
- Experiment registry (all experiments, all time)
- Active experiments dashboard
- Completed experiment reports with learnings
- Conflict alerts (overlapping tests)
- Monthly experiment velocity report

## Boundaries
- ✅ Logs and tracks all experiments
- ✅ Maintains experiment history
- ✅ Records results and learnings
- ✅ Flags conflicts
- ❌ Does NOT design experiments (owned by relevant team)
- ❌ Does NOT analyze results (owned by test-results-analyzer)
- ❌ Does NOT decide winners (owned by test-results-analyzer)
- ❌ Does NOT implement variants (owned by engineering/marketing)
