

Welcome to Solving Problems with Data!
======================================

Hello, and welcome to the course site for Duke IDS 701!

Few fields have shown as much promise to address the world's problems as data science. At the same time, however, recent years have also made clear that today's global challenges will not be met by simply "throwing data science at the problem" and hoping things will work out. Even in business, where many assume that Artificial Intelligence is a sure ticket to profits, a major recent study found `only 11% of businesses that had piloted or employed Artificial Intelligence had reaped a sizeable return on their AI investments. <https://www.wired.com/story/companies-rushing-use-ai-few-see-payoff/>`__

How, then, should a burgeoning data scientist approach this field full of such promise but also so many pitfalls? And why have so many data science endeavors failed to deliver on their promise?

The answer lies — at least in significant part — in a failure to provide students with a systematic approach to bringing the techniques learned in statistical modeling and machine learning courses to bear on real-world problems. Data science curricula usually begin with coding, statistics, and model evaluation techniques. All too often, however, that's where they stop. But while the hardest part of data science *classes* is often fitting a model well or getting a good AUC score, the hardest part of being an effective *professional* data scientist is ensuring that the models being fit and the results being interpreted actually solve the problem that motivated you (or your stakeholder) in the first place.

This class is designed to fill this gap. Through exercises, case studies, and projects, students will develop a *systematic* understanding of how to approach and manage data science projects from conception through delivery and adoption. It will provide a unified perspective on how the perspectives and tools learned in other courses complement one another, and *when* different approaches to data science are most appropriate. 

In addition, this course will also provide an in-depth introduction into *causal inference* — the practice of answering causal questions. Given the interests of MIDS students, this introduction will focus heavily on experiments and A/B testing, but will also cover the use of observational data (data that did not come from an experiment that employed random assignment to treatment) for answering causal questions.


Pre-Requisites for Non-MIDS Students
------------------------------------
This course is primarily designed for students in the Duke Masters in Interdisciplinary Data Science (MIDS) program, but students from other programs are more than welcome if they have the appropriate pre-requisite training. Data Science is a fundamentally interdisciplinary field, so the more perspectives we have represented in the classroom the better!

This course will assume that enrolled students have a good grasp of inferential statistics and statistical modeling (e.g. a course in linear models), though no prior experience with causal inference is expected. In addition, MIDS students will be taking a concurrent course in applied machine learning, so incoming students will also be expected to have some basic experience with machine learning or be concurrently enrolled in an applied machine learning course.

This course will also assume students are comfortable manipulating real-world data in either Python or R. The substantive content of this course is language-independent, but because students will be required to work on their projects in teams, comfort with Python will be required to facilitate collaboration (MIDS students are, generally, "bilingual" in R and Python, but have a strong preference for Python, and it's hard to write problem sets to accommodate multiple languages).

Finally, students will also be expected to be comfortable collaborating using git and github. If you meet the other requirements for this course but are not familiar with git and github, this is a skill you should be able to pickup on your own in advance of the course without too much difficulty. You can read more about `git and github here <https://www.practicaldatascience.org/html/git_and_github.html>`_. The `Duke Center for Data and Visualization Science <https://library.duke.edu/data/>`_ also hosts git and github workshops if you are a Duke student.


Syllabus
--------

To learn more about the course, please `read the course syllabus available here. <https://github.com/nickeubank/unifyingdatascience/raw/master/syllabus/Syllabus_UnifyingDataScience.pdf>`_ and see a `preliminary schedule and texts we'll be using here <class_schedule.rst>`_. Note that our schedule is subject to change, but should give you a good sense of the material we will cover.


.. toctree::
   :maxdepth: 2
   :hidden:

   CLASS SCHEDULE <class_schedule>

.. toctree::
   :maxdepth: 2
   :caption: Causal Inference
   :hidden:

   Limitations of ATE <limitations_of_ATE>
   Internal v. External Validity <internal_v_external_validity>
   Evaluating A Real Study <evaluating_real_studies>
   Beyond AB Testing <causal_inference_beyond_ab_testing>
   Matching (Why) <matching_why>
   Matching (How) <matching_how>
   Indicator Variables <interpreting_indicator_vars>
   Fixed Effects (FEs) <fixed_effects>
   FEs & Causality <fixed_effects_and_causal_inference>
   FEs & Hierarchical Models <fixed_effects_v_hierarchical>


.. toctree::
   :maxdepth: 2
   :caption: Data Science Project Design
   :hidden:

   Backwards Design <backwards_design>
   Taxonomy of Questions <taxonomy_of_questions>
   From Problems to Questions <moving_from_problems_to_questions>
   Discretion and Description <descriptive_questions.ipynb>
   Ethical Machine Learning <ethical_ml_recommendations.ipynb>
   Writing for Lay Audiences <writing_to_stakeholders>
