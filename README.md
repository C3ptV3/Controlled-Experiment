
Quality Management and Experimental 
Software Engineering






Report from controlled experiment: 
Evaluating the productivity of TDD method against TAC




Authors:
Elchin Habibov
Davut Aslan











Poznan, 15.01.2020
Introduction
This report presents design and summarizes results of the experiment Evaluating the productivity of TDD method against TAC. The experiment was a part of the project realized in the frame of Quality Management and Experimental Software Engineering classes at Poznan University of Technology.
Experiment definition
The goal of the experiment was to:
Analyze Test Driven Development and Test After Coding
With the purpose of comparing
With respect to performances of testing
From the point of view of the developers
In the context of a group of students.

The research goal consist of this research question:
 	• Is TDD more productive than TAC from 
 	of the testing? In the case, the product is intended
as the set of test cases and correct code; the code is
considered correct if all the related tests succeed. Thus,
‘productivity’ is seen as the efficiency in producing test
cases and correct code.
Experiment design
Hypotheses 
The experiment aimed at testing the following null hypotheses.
H0: there is no difference in the productivity between TDD and
TAC.
H1: there is  difference in the productivity between TDD and
TAC.

Variables and confounding factors
Independent variables
Programming methods:
•	TDD –Test Driven Development Method
•	TAC-Test After Coding Method
Dependent variable
MeanTime -It is the mean time for writing and executing a test suite. 
Participants
The 8 subjects were selected among a set of students with comparable skills: they had 4 years of experience in using c and in computer programming.
Objects 
The subjects were required to solve simple “String manipulation” problem. The programming language was C, while “onlinegdb.com” compiler  was chosen as development environments. For precision’s sake, the subjects were required to write the code and the test suites for the requirements.
Test definition
Subjects was divided in 2 groups randomly to perform the task with TDD and TAC method.
Experiment operation
Prepared instrumentation
As the subjects had no previous experience on TDD, we performed introductory  explanation of the method before the experiment.
Execution
The experiment consisted 1 run: run lasted approximately 1 hour. 
• in the run subjects had to write down
o the start time; and
o end time, which takes into account when the test is
overcome, i.e. when every bug is detected and the test is
passed without any failure.
At the end of the run, the data about the time collected from each subject.
Analysis and interpretation
Descriptive statistics
The total time for performing run of each subject(Independently from each other.)
TDD	TAC
35	18
40	24
45	30
47	32

Quick summary of the data. The important factor for the experiment is MeanTime, as stated.

      TDD             TAC      
 Min.   :35.00   Min.   :18.0  
 1st Qu.:38.75   1st Qu.:22.5  
 Median :42.50   Median :27.0  
 Mean   :41.75   Mean   :26.0  
 3rd Qu.:45.50   3rd Qu.:30.5  
 Max.   :47.00   Max.   :32.0 

Hypotheses testing

H0: there is no difference in the productivity between TDD and
TAC.
H1: there is  difference in the productivity between TDD and
TAC.
p-level was fixed at 0.05.
To prove hypotheses Welch Two Sample t-test performed.

data:  exp_data$TDD and exp_data$TAC
t = 3.7944, df = 5.8487, p-value = 0.004735
alternative hypothesis: true difference in means is greater than 95 percent confidence interval:
 7.646727      Inf
sample estimates:
mean of x mean of y 
    41.75     26.00 

MeanTime p-value=0.004735 There is evidence that TDD requires more time in average than TAC. And proves H1
Interpretation of the results
The statistical test of hypotheses produced the following results: 
• there is evidence that TDD requires more time than TAC.
Threats to validity
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


Conclusions
TDD is a practice which prescribes to write and change the code
of a class’ method only on the basis of the correspondent unit test’
results.
Although TDD is considered a ‘development practice’ rather than
a testing practice, it is actually twofold, because it includes both
coding and testing aspects in a tightly interleaved process. Since
TDD is a practice per se and it might be used also independently
from the other agile practices and in other kinds of software
processes, we wondered if and when TDD can be preferred to the
traditional TAC.
We believe that TDD is more time consuming than TAC, but
leads developer to design more precise and more accurate test cases.

