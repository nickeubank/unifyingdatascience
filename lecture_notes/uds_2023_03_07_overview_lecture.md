# Overview Lecture of Causal Inference

OK, so what's up?

## Solving Problems

- Specify problem
- Articulate question which, if answered, would help solve problem
  - Exploratory Questions: Prioritization
  - Passive-Predictive Questions: Automation or targeting
  - Causal Questions: here we go!

## Causal Questions

Want to manipulate something in the world, and want to know the effect of our actions.

In other words, we want an estimate of ATE.

### Potential Outcomes

What we want: E(Y_{T=1}) - E(Y_{T=0})
What we can measure: E(Y_{T=1}|D=1) - E(Y_{T=0}|D=0)

**IF** E(Y_{T=0}|D=0) = E(Y_{T=0}|D=1)
    - No baseline differences
    - e.g., in a world without treatment, outcomes would be the same.

**THEN**:

What we can measure               == Treatment effect for treated
E(Y_{T=1}|D=1) - E(Y_{T=0}|D=0)   == E(Y_{T=1}|D=1) - E(Y_{T=0}|D=1)
                                  == ATT

In addition, if treatment response is same for treated (D=1)
and untreated (D=0), then ATT == ATE
