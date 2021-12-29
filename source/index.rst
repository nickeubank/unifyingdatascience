

Welcome to Unifying Data Science!
=================================

Hello, and welcome to the course site for Duke IDS 701!

The first portion of the course will provide an application-focused introduction to *causal inference*, the art and science of using statistical data to make causal statements about the world. Our approach will be rooted in the potential outcomes framework, and will cover a range of methods of statistical inference including randomized experiments, pre-post analysis, differences-in-differences, and instrumental variables. In addition, we will also discuss concepts like the distinction between internal and external validity, and the limitations of estimating Average Treatment Effects. 

In the second portion of the course, we will turn to the fundamental task of the data scientist: executing a full data science project from conceptualization through planning and execution. In particular, we will introduce a question-first, backwards design framework for systematically designing a data science project. Through exercises, students will practice each step of this approach, from working with stakeholders to properly articulate the problem they are seeking to address, to picking a question (which, if answered, will help the stakeholder solve their problem), selecting the appropriate methodological approach to answering that question, and developing a concrete strategy for generating an answer.

In addition to completing a number of exercises related to project design, over the semester students will conduct a complete data science project themselves. Data science is a fundamentally applied field, and there is no substitute for learning to put these project design principles into action through practice. These projects will be developed incrementally over the course of the semester with instructor guidance. By the end of the semester, students will have picked a topic area, developed a (tractable) question, decided what an answer to that question would actually look like, developed a work plan for generating that answer, and executed and presented their project, and then iterated the project based on feedback from their initial presentation. For MIDS students, this will serve as a "capstone-project with training wheels" to prepare students for their second-year Capstone projects with external partners. And this project should provide all students with a portfolio piece they can present to potential future employers. 

Throughout the course, we will also be consistently returning to a few themes, chief among them the importance of developing a skeptical mindset. This is a core data science skill, but one that students do not always have the opportunity to practice. In this course, we will discuss *and practice* approaching our data, our code, our statistical models, our problem statements, and the work of others from a constructive but skeptical perspective.

Pre-Requisites for Non-MIDS Students
------------------------------------

This course is primarily designed for students in the Duke Masters in Interdisciplinary Data Science (MIDS) program, but students from other programs are more then welcome if they have the appropriate pre-requisite training. Data Science is a fundamentally interdisciplinary field, so the more perspectives we have represented in the classroom the better!

This course will assume that enrolled students have a good grasp of inferential statistics and statistical modelling (e.g. a course in linear models), though no prior experience with causal inference is expected. In addition, MIDS students will be taking a concurrent course in applied machine learning, and so incoming students will also be expected to have some basic experience with machine learning, or be concurrently enrolled in an applied machine learning course.

This course will also assume students are comfortable manipulating real-world data in either Python or R. The substantive content of this course is language-independent, but because students will be required to work on their projects in teams, comfort with one of these two languages will be required to facilitate collaboration (Note that while MIDS students are, generally, "bilingual" in R and Python, they generally prefer Python, so life will be a little easier if you have a background in pandas). Where code examples are provided in class, they will use Python (`pandas`), but both the instructor and our TAs are also capable of providing support in R.

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
   :caption: Data Science Concepts
   :hidden:

   Taxonomy of Questions <taxonomy_of_questions>
   From Problems to Questions <moving_from_problems_to_questions>
   Discretion and Description <descriptive_questions.ipynb>
   Ethical Machine Learning <ethical_ml_recommendations.ipynb>
   Writing for Lay Audiences <writing_to_stakeholders>

.. toctree::
   :maxdepth: 2
   :caption: Causal Inference
   :hidden:

   Limitations of ATE <limitations_of_ATE>
   Internal v. External Validity <internal_v_external_validity>
   Evaluating A Real Study <evaluating_real_studies>
   Matching (Why) <matching_why>
   Matching (How) <matching_how>
   Indicator Variables <interpreting_indicator_vars>
   Fixed Effects (FEs) <fixed_effects>
   FEs & Causality <fixed_effects_and_causal_inference>
   FEs & Hierarchical Models <fixed_effects_v_hierarchical>
