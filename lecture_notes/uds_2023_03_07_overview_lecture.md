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
and untreated (D=0),
E(Y_{T=1}|D=1) - E(Y_{T=0}|D=1) == E(Y_{T=1}|D=0) - E(Y_{T=0}|D=0)
then ATT == ATE

Note that this last issue is more like a *generalization* problem. ATT *is* a real treatment effect,
it just may not generalize perfectly to the control population.

**SO HOW DO WE GET E(Y_{T=0}|D=0) = E(Y_{T=0}|D=1)** ??

### Experiments / RCTs / AB Testing

Randomize! LLN --> control and treatment look the same.

Thus, E(Y_{T=0}|D=0) = E(Y_{T=0}|D=1)
And, automatically, E(Y_{T=1}|D=1) - E(Y_{T=0}|D=1) == E(Y_{T=1}|D=0) - E(Y_{T=0}|D=0)

ATE! Provided a few other assumptions (SUTVA, compliance, etc.)

### Regression

Suppose E(Y_{T=0}|D=0) \neq E(Y_{T=0}|D=1), BUT we think we know why.

For example, suppose that ....

Then *after conditioning on X*, we can get to:

E(Y_{T=0}|D=0, X) = E(Y_{T=0}|D=1, X)

And our estimates are causal! (Though ATT)

But our estimates will only be causal _in so far as we can directly measure
the factors that matter_.

**Example:**

For example, suppose two kinds of dog food bags: big bags and small.
Dog food with free shipping generates more revenue per week. But
we also know that:

- (a) people prefer smaller bags of dog food, and
- (b) sellers offer free shipping more often for smaller dog food.

revenue | free_shipping | size
- --------------------------- -
100     |  No           | 10
150     |  Yes          | 10
145     |  Yes          | 10
50      |  No           | 30
45      |  No           | 30
100     |  Yes          | 30

E(Y_{T=0}|D=0) = 65
E(Y_{T=1}|D=1) = 131.67

E(Y_{T=1}|D=1) - E(Y_{T=0}|D=0) = 66.67

But we can see that E(Y_{T=0}|D=0) != E(Y_{T=0}|D=1),
as D=1 tends to be small bag (2/3), D=0 tends to be big (2/3).

But as regression:

```
 coef std err t P>|t| [0.025 0.975]
Intercept 123.3333 3.879 31.796 0.000 110.989 135.678
free_shipping[T.True] 50.0000 2.887 17.321 0.000 40.813 59.187
bag_size -2.5000 0.144 -17.321 0.000 -2.959 -2.041
```

E(Y_{T=1}|D=1, bag_size) - E(Y_{T=0}|D=0, bag_size) = 50

### Fixed Effects

Suppose we have multiple observations from the same entity (say, brand).
 Maybe we don't need to specify all the things that make our entities
 different explicitly (brand image, customer satisfaction, age, etc.)
 instead we can just add fixed effects.

### Matching

Functional forms are a b*tch.

### FE to Diff-in-Diff

pre-post (e.g., product FE for products that moved from paid to free): revenue up!

But what if that was just the pandemic?
