Quality Management and Experimental
Software Engineering







## Report from controlled experiment:

## Evaluating the productivity of TDD method against TAC





Authors:

Elchin Habibov

Davut Aslan











Poznan, 15.01.2020

# Introduction

This report presents design and summarizes results of the experiment **Evaluating the productivity of TDD method against TAC**. The experiment was a part of the project realized in the frame of Quality Management and Experimental Software Engineering classes at Poznan University of
#
[ANNOTATION:

BY &#39;Mirosław Ochodek&#39;
ON &#39;2014-11-24T16:01:00&#39;MO
NOTE: &#39;You can extend the introduction if you like.&#39;]
Technology.

# Experiment
#
[ANNOTATION:

BY &#39;Mirosław Ochodek&#39;
ON &#39;2014-11-24T16:03:00&#39;MO
NOTE: &#39;You should define the goal of the experiment here, e.g. using the template known from GQM&#39;]
definition

The goal of the experiment was to:

# _Analyze Test Driven Development and Test After Coding_

# _With the purpose of comparing_

# _With respect to performances of testing_

# _From the point of view of the developers_

# _In the context of a group of students._

The research goal consist of this research question:

  • Is TDD more productive than TAC from

  of the testing? In the case, the product is intended

as the set of test cases and correct code; the code is

considered correct if all the related tests succeed. Thus,

&#39;productivity&#39; is seen as the efficiency in producing test

cases and correct code.

# Experiment design

##
#
[ANNOTATION:

BY &#39;Mirosław Ochodek&#39;
ON &#39;2014-11-24T16:07:00&#39;MO
NOTE: &#39;Describe a priori considered hypotheses of you study.&#39;]
Hypotheses

The experiment aimed at testing the following null hypotheses.

H0: there is no difference in the productivity between TDD and

TAC.

H1: there is  difference in the productivity between TDD and

TAC.

## Variables and confounding
#
[ANNOTATION:

BY &#39;Mirosław Ochodek&#39;
ON &#39;2014-11-24T16:08:00&#39;MO
NOTE: &#39;Define:&#39;
NOTE: &#39;Independent variables (possible values, measurement scales)&#39;
NOTE: &#39;Dependent variables (possible values, measurement scales)&#39;
NOTE: &#39;Confounding factors (how they were controlled)&#39;]
factors

Independent variables

Programming methods:

- TDD –Test Driven Development Method
- TAC-Test After Coding Method

Dependent variable

MeanTime -It is the mean time for writing and executing a test suite.

## Participants
#
[ANNOTATION:

BY &#39;Mirosław Ochodek&#39;
ON &#39;2014-11-24T16:12:00&#39;MO
NOTE: &#39;Describe the participants selection strategy, the number of participants and any of their characteristics important to the study. &#39;]

The 8 subjects were selected among a set of students with comparable skills: they had 4 years of experience in using c and in computer programming.

##
#
[ANNOTATION:

BY &#39;Mirosław Ochodek&#39;
ON &#39;2014-11-24T16:14:00&#39;MO
NOTE: &#39;Describe the objects of the experiment – the things that participants worked on, e.g., piece of code they were given, etc.&#39;]
Objects

The subjects were required to solve simple &quot;String manipulation&quot; problem. The programming language was C, while &quot;onlinegdb.com&quot; compiler  was chosen as development environments. For precision&#39;s sake, the subjects were required to write the code and the test suites for the requirements.

## Test
#
[ANNOTATION:

BY &#39;Mirosław Ochodek&#39;
ON &#39;2014-11-24T16:17:00&#39;MO
NOTE: &#39;Discuss how variables, participants and objects were assigned together. E.g., participants were planned to be divided into two groups : G1 used \&lt;value of independent variable\&gt; and G2 was supposed to use \&lt;value of independent variable\&gt; … to [do something] with \&lt;object\&gt; .&#39;]
definition

Subjects was divided in 2 groups randomly to perform the task with TDD and TAC method.

# Experiment operation

## Prepared
#
[ANNOTATION:

BY &#39;Mirosław Ochodek&#39;
ON &#39;2014-11-24T16:19:00&#39;MO
NOTE: &#39;Describe any instrumentation given to the participants. This includes introductory lecture, any handouts, any sheets to fill, etc. (of course both in manual and electronic form.&#39;]
instrumentation

As the subjects had no previous experience on TDD, we performed introductory  explanation of the method before the experiment.

##
#
[ANNOTATION:

BY &#39;Mirosław Ochodek&#39;
ON &#39;2014-11-24T16:20:00&#39;MO
NOTE: &#39;Say when the experiment was executed. How it looked like (give steps). State how long each step taken. State how the data was collected.&#39;]
Execution

The experiment consisted 1 run: run lasted approximately 1 hour.

• in the run subjects had to write down

o the start time; and

o end time, which takes into account when the test is

overcome, i.e. when every bug is detected and the test is

passed without any failure.

At the end of the run, the data about the time collected from each subject.

# Analysis and interpretation

## Descriptive
#
[ANNOTATION:

BY &#39;Mirosław Ochodek&#39;
ON &#39;2014-11-24T16:23:00&#39;MO
NOTE: &#39;In this section you should:&#39;
NOTE: &#39; Discuss the completeness of the data&#39;
NOTE: &#39; &quot;Visualize the data&quot; – either present some plots presenting the distributions of the results or give descriptive statistics&#39;
NOTE: &#39; Identify and analyze the outliers&#39;]
statistics

The total time for performing run of each subject(Independently from each other.)

TDD        TAC

35        18

40        24

45        30

47        32

Quick summary of the data. The important factor for the experiment is MeanTime, as stated.

      TDD             TAC

 Min.   :35.00   Min.   :18.0

 1st Qu.:38.75   1st Qu.:22.5

 Median :42.50   Median :27.0

  **Mean   :41.75**   **Mean   :26.0**

 3rd Qu.:45.50   3rd Qu.:30.5

 Max.   :47.00   Max.   :32.0

## Hypotheses
#
[ANNOTATION:

BY &#39;Mirosław Ochodek&#39;
ON &#39;2014-11-24T16:29:00&#39;MO
NOTE: &#39; Here you should:&#39;
NOTE: &#39; justify the choice of statistical tests used &#39;
NOTE: &#39; present the hypotheses (null and alternative)&#39;
NOTE: &#39; show the results of the tests&#39;
NOTE: &#39;perform power analysis (especially important if you were not able to reject Null hypothesis!!!!!)&#39;
NOTE: &#39;&#39;]
testing

H0: there is no difference in the productivity between TDD and

TAC.

H1: there is  difference in the productivity between TDD and

TAC.

p-level was fixed at 0.05.

To prove hypotheses Welch Two Sample t-test performed.

data:  exp\_data$TDD and exp\_data$TAC

t = 3.7944, df = 5.8487, p-value = 0.004735

alternative hypothesis: true difference in means is greater than 95 percent confidence interval:

 7.646727      Inf

sample estimates:

mean of x mean of y

    41.75     26.00

MeanTime p-value=0.004735 There is evidence that TDD requires more time in average than TAC. And proves H1

## Interpretation of the
#
[ANNOTATION:

BY &#39;Mirosław Ochodek&#39;
ON &#39;2014-11-24T16:27:00&#39;MO
NOTE: &#39;interpret the results – explain what the obtained results indicate&#39;]
results

The statistical test of hypotheses produced the following results:

• there is evidence that TDD requires more time than TAC.

# Threats to
#
[ANNOTATION:

BY &#39;Mirosław Ochodek&#39;
ON &#39;2014-11-24T16:29:00&#39;MO
NOTE: &#39;Discus:&#39;
NOTE: &#39;Conclusion validity&#39;
NOTE: &#39;Internal validity&#39;
NOTE: &#39;Construct validity&#39;
NOTE: &#39;External validity&#39;
NOTE: &#39;&#39;]
validity

The following issues have been dealt with:

• Differences among subjects. Using a within-subjects

design, error variance due to differences among subjects

was reduced. The subjects had same amount of experience in C

programming language and environment.

• Persistence effects. In order to avoid persistence effects,

the experiment was run with subjects who had never

done a similar experiment.

• Subject motivation. Students showed a great interest

in taking part to a scientific experiment. They were

pleased to exercise TAC and TDD which could

bring benefits to their daily work.

• Other factors. Plagiarism and influence among subjects

were controlled by supervising the run.

# Conclusions

TDD is a practice which prescribes to write and change the code

of a class&#39; method only on the basis of the correspondent unit test&#39;

results.

Although TDD is considered a &#39;development practice&#39; rather than

a testing practice, it is actually twofold, because it includes both

coding and testing aspects in a tightly interleaved process. Since

TDD is a practice per se and it might be used also independently

from the other agile practices and in other kinds of software

processes, we wondered if and when TDD can be preferred to the

traditional TAC.

We believe that TDD is more time consuming than TAC, but

leads developer to design more precise and more accurate test cases.
