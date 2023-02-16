## Terms

It is a bit confusing that A/B testing is introduced as causal inference with “observational” data in the reading because data gathered by A/B testing can be considered as rather “experimental”. In my understanding, observational data means some data collected by observing natural phenomena which have nothing to do with any artificial settings. But, A/B testing is definitely to put users into two or more settings and force them to experience different things.

Charlotte:

A/B testing but I bet it's the same thing as RCTs

## Ethics

Dany:

One thing I was curious about was the concern of legality or ethics of A/B testing in certain situations. It seems like in many cases these concerns can be somewhat nebulous. Showing some users one thing and other users something else would in my opinion in most cases result emotional manipulation. I was curious what efforts if any are taken to define what constitutes user manipulation that is too extreme and unethical.

Xiaoquan:

How do we measure the ethics of A/B testing? Since the Facebook experiment cost Facebook a lot of good will, does that mean it's okay to do experiments like that? Or,  since all experiments somehow impact people's daily lives, it's possible that someone views a certain experiment as harmful but others may not. How do we properly evaluate those things?

## When A/B

The first reading discusses the limitations of A/B testing, and why it is not always feasible, like the Netflix example (talking about an alternative like Quasi experiment), but which cases would be ideal to conduct A/B testing? Can we have some examples of which scenario we should consider A/B testing and how to actually conduct it? I know the reading mentions that A/B testing tools are prevalent nowadays, but I still consider myself at the stage of learning how to employ A/B testing, especially in tech industry settings. I wonder if we can go over an example together in class.

## 80/20

Kashaf:

Both readings for this lecture made me ponder about a critical question: does establishing causality always matter in the practical world? While establishing causality helps in understanding relationships between different variables and making data-driven decisions, would it be the best approach in real world settings? As discussed in the "Beyond The Experiment" reading, A/B testing is not always feasible, and the "Mastering Metrics" reading also discusses how measuring omitted variable bias can only help us identify relationships for omitted variables that are actually observable, it is difficult to always establish causation in a real-world setting, especially when business or stakeholders have less time and resources. In my experience of working at a startup (which are known to have limited time and resources), establishing causation was considered an expensive and time-consuming task, and instead the focus was on the 80-20 rule also known as the Pareto Principle, which asserts that if you know that 80% of the outcomes result from 20% of all inputs for any given event, it is enough to make a decision. For instance, at my company running A/B tests meant designing product solutions in the app which allowed us to segment customers properly - this was both expensive and was taking months to deploy, and it was not profitable to wait for these product solutions to test out new changes in a market that was fiercely competitive and quickly evolving. A lot of companies now focus on lean decision making, where the focus is on making quick decisions based on the 80-20 rule and then iterating to improve it before you scale. In a world which is becoming more fast-paced, resource-constraint, and competitive, is it reasonable to invest time in establishing causation? If no, are there any other adaptive methods that can offer the same level of robustness?

## Why measure?

Genesis:

In the MM reading, why is it necessary to calculate the value for Omitted Variable Bias? Isn't that bias represented by the value of the control variable in the long formula already? What's the value in getting a precise number of the OVB? Additionally, in the 5-student example of the private-public income comparison, the reading said that because group C and D have only homogenous groups, the have negligible impact on our treatment estimates. However, if you input those variables into a regression, wouldn't the observations in group C and D nonetheless influence estimates of the treatment parameter and the other parameters?

Nick:

One thing I found confusing is understanding estimation of the omitted variables bias.  After all, the omitted variable bias is based on understanding the impact of variables that are omitted, and therefore, unlike in the reading where omitting variables and calculating the results is possible, in a real example, you don't know what you've omitted.  How do you assume analyzing your model's sensitivity provides insight into models that were missed in your model?

## Machine learning relevance

Pooja:

How do the concepts of regression we learn in machine learning apply to the regression used for causal inference? Addition of variables other than the treatment variable on the right hand side increases confidence in and better estimates the response variable but does it overfit the data used for the regression? Does this hurt the generalizability of the inference and does it have anything to do with external validity?

## At Risk

Zhonglin:

I have very in-depth feelings about at-risk contracting in my previous experiences. In situations when we only want to measure the effect of a large, single intervention, since the reading holds the viewpoint that A/B testing has been limited, should we use casual inference under these circumstances? Or should we just carefully consider the confounders in our experiments.

## In-house AB?

Susanna:

I don't understand how platforms can have an in house A/B testing feature. To my understanding, which is extremely limited, each A/B test is very individualized and has a variety of different characteristics like the treatments, the response variables or metrics to measure response, sample size, time, location, demographics of those in the sample, etc. Is it possible because, as we spoke about in class, the law of large numbers makes it so that time, location, and demographics of users kind of even out as n -> infinity? So, in the platform there's a built in minimum size of sample so that stratification and mindfulness of demographics is not necessary?

While Googling to figure out how these features work, I found out that A/A testing exists; A/A testing is showing the same treatment to two different groups. I'm reading that this ensures that the A/B test is statistically fair; I don't really understand how this makes it fair? Say, we show webpage A to groups A and C, then we show webpage B to groups B and D. We find that the difference in response to webpage A is not statistically significant, meaning that groups A and C had the same response to webpage A. We also find the same for webpage B for groups B and D. This seems like an example of A/A testing?

Now, say that webpage A is the website's layout in its current state and webpage B is a redesign of webpage A. How does knowing that the two groups had the same response to the same webpage make the experiment more fair? Is it that we are somewhat controlling for baseline effects between two groups? Like, making sure that one of the two groups didn't have a weird, abnormal distribution of a certain group? But aren't there better methods for ensuring that?
