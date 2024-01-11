- Thursday / Tuesday

- Fairness
  - Vicki: What is the difference between bias and fairness or to be explicit, are unfairness and bias the same? Why is fairness in AI important? Does fairness mean equality?
-  Robert: I didn't quite understand Warmerdam's measure for bias. If I interpreted his explanations correctly, he's saying that if a categorical variable is unbiased, then the expected predicted values of the classes should be the same. This seems problematic to me. If a variable has predictive power, then we'd expect the predicted values for two values to be different. By removing variables that are "biased" according to Warmerdam's definitions, how do we make sure that we're not just removing variables that 1) seem sensitive from a logical reasoning perspective, and 2) also have predictive power?

- Adversarial Users / Misalignment
  - https://www.smbc-comics.com/comic/fuel-2
- Lucas Critique
  - Jaya: While it is fascinating to read about the problems that come with AI systems, I wonder if we can incorporate rule-based system within our causal inference project? On the same note, the question I think of - are these problems only seen in AI systems (prediction) or are these also ubiquitous in causal inference systems? 

Questions:

- Rachel: I understand how models can be unfair and biased, but what are the key indicators to seeing this? I know that once we see the model's results and interpret them we can see how it reacts to different groups of people, but we only know this after the model is created. Is there a key indicator, other than just EDA, that tells us if the model is biased and whether we should implement fairness into the model in the first place?
- Raza: To me, auto-grading essays does not seem like a problem that should be solved by machine-learning/artificial intelligence, due to everything I have read about it—at least, not right now. This one, to me, seems relatively easy. But, I think a lot of other algorithms are in a much more grey area, especially when outcomes by “fairness” cannot be easily obtained. How do we know when to quit? When should we stop pursuing a “smart” solution because of potential (or realized) harm?
- Athena: In the video, Vincent Warmerdam mentioned that predict_proba is a prediction of probability but not a prediction of certainty (8:12 ish). Could you please explain the difference between probability and certainty? 

