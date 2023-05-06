Download Link: https://assignmentchef.com/product/solved-ece523-homework2
<br>
<h1>1           Linear Classifier with a Margin</h1>

Show that, regardless of the dimensionality of the feature vectors, a data set that has just two data points, one from each class, is sufficient to determine the location of the maximum-margin hyperplane. Hint #1: Consider a data set of two data points, <strong>x</strong><sub>1 </sub>∈ C<sub>1 </sub>(<em>y</em><sub>1 </sub>= +1) and <strong>x</strong><sub>2 </sub>∈ C<sub>2</sub>

(<em>y</em><sub>2 </sub>= −1) and set up the minimization problem (for computing the hyperplane) with appropriate constraints on <strong>w</strong><sup>T</sup><strong>x</strong><sub>1 </sub>+ <em>b </em>and <strong>w</strong><sup>T</sup><strong>x</strong><sub>2 </sub>+ <em>b </em>and solve it. Hint #2: This can be formed as a constrained optimization problem.

arg min <strong>w</strong>∈R<em><sup>p</sup></em>

Subject to: (some constraint)

What is <strong>w</strong>? <em>b</em>? Hint: What are the constraints? How did we solve the constrained optimization problem in Fisher’s linear discriminate (see Linear Models Lecture Notes or constrained optimization from Calculus)?

<h1>2           Linear Regression with Regularization</h1>

In class we derived and discussed linear regression in detail. Find the result of minimize the loss of sum of the squared errors; however, add in a penalty for an <em>L</em><sub>2 </sub>penalty on the weights. More

formally,

argmin <strong>w</strong>

How does this change the solution to the original linear regression solution? What is the impact of adding in this penalty?

Write your own implementation of logistic regression and implement your model on either realworld (see Github data sets: <a href="https://github.com/gditzler/UA-ECE-523-Sp2018/tree/master/data">https://github.com/gditzler/UA-ECE-523-Sp2018/tree/master/ </a><a href="https://github.com/gditzler/UA-ECE-523-Sp2018/tree/master/data">data</a><a href="https://github.com/gditzler/UA-ECE-523-Sp2018/tree/master/data">)</a>, or synthetic data. If you simply use Scikit-learn’s implementation of the logistic regression classifier, then you’ll receive zero points. A full 10/10 will be awarded to those that implement logistic regression using the optimization of cross-entropy using stochastic gradient descent.

<h1>3           Density Estimation</h1>

The ECE523 Lecture notes has a function for generating a checkerboard data set. Generate checkerboard data from two classes and use any density estimate technique we discussed to classify new data using

where is your estimate of the posterior given you estimates of using a density estimator and <em>p</em>b<em><sub>Y </sub></em>(<em>y</em>) using a maximum likelihood estimator. You should plot <em>p</em><sub>b</sub><em>X</em><sub>|<em>Y </em></sub>(<em>x</em>|<em>y</em>) using a pseudo color plot (see <a href="https://goo.gl/2SDJPL">https://goo.gl/2SDJPL</a><a href="https://goo.gl/2SDJPL">)</a>. Note that you must model <em>p</em>b<em><sub>X</sub></em>(<em>x</em>), <em>p</em><sub>b</sub><em>Y </em>(<em>y</em>), and <em>p</em>b<em><sub>X</sub></em><sub>|<em>Y </em></sub>(<em>x</em>|<em>y</em>). Note that <em>p</em><sub>b</sub><em>X</em>(<em>x</em>) can be calculated using the Law of Total Probability.

<h1>4           Conceptual</h1>

The Bayes decision rule describes the approach we take to choosing a class <em>ω </em>for a data point <strong>x</strong>. This can be achieved modeling <em>P</em>(<em>ω</em>|<strong>x</strong>) or <em>P</em>(<strong>x</strong>|<em>ω</em>)<em>P</em>(<em>ω</em>)<em>/P</em>(<strong>x</strong>). Compare and contrast these two approaches to modeling and discuss the advantages and disadvantages. For the latter model, why might knowing <em>P</em>(<strong>x</strong>) be useful?