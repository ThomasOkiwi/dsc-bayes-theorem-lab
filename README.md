

## Bayesian Statistics - Introduction
  
## Introduction
In this section, you'll investigate the Bayesian statistical framework. Bayesian statistics are an alternative perspective to classical Frequentist approaches which you've seen thus far. Bayesian statistics applies reasoning to unknown probabilities in a manner in which the Frequentist approach does not allow.
## Thomas Bayes
Bayesian statistics owes its name to the famous mathematician Thomas Bayes. Born (sometime) in the early 1700s, he bucked many academic traditions of his time due to his families religious beliefs. Cambridge and Oxford were known for the most prestigious mathematics of the time, but Bayes was a Presbytarien barring him from these universities which had ties to the Church of England.
## Bayes' theorem
Bayes' theorem is a method for rewriting conditional probabilities. The formula is:
 
In the following lessons, you'll learn more about two traditional interpretations of this formula. The first provides an intuitive understanding, viewing the numerator as the probability of both A and B occuring:
 
This should make perfect sense: the probability that A is true, given B is true, is the probability that A and B are both true, divided by the probability that B was true in the first place.
The second interpretation of Bayes theorem leads straight into the Bayesian statistical framework itself, bringing about discussions of priors, likelihoods, and posterior probabilities.

## Bayesians vs Frequentists
  
Introduction
Up until now, all of the statistical theory you have encountered has been through the lens of a Frequentist. This has included discussions of z-tests, t-tests, p-values, and ANOVA; all are from the Frequentist perspective. In this lesson, you'll start to explore an alternative perspective donned by Bayesians.
## Objectives
You will be able to:
- Compare the Bayesian v. Frequentist statistical frameworks
## Philosophical Interpretations

A natural place to start when outlining the differences between Bayesians and Frequentists is to talk of their interpretation of probability itself. For Frequentists, the probability of an event is the limit of the rate of occurrences of the event if the same scenario including context and assumptions were repeated ad infinitum. In contrast, Bayesians interpret probability as the level of confidence, or belief, in a particular event occurring. In many ways, this makes a more natural interpretation for rare events that cannot possibly reoccur in the same context and circumstances.
## Practical Implications

The practical implications of Bayesians versus Frequentists rest upon making assumptions about unknown quantities. In the Bayesian framework, you make assumptions about unknown variables which you are attempting to estimate. For example, you might assume that the number of individuals who will buy a product can be represented by a binomial variable with parameter   . In contrast, the Frequentist perspective does not allow embedding of prior beliefs such as this into statistical experiments and analyses.

## Bayes' Theorem
  
### Introduction
Bayes theorem is an indispensable law of probability, allowing you to deductively quantify unknown probabilities. The theory rests upon conditional probability. Let's take a look at it in practice.
Objectives
You will be able to:
•	Define Bayes' theorem in relation to conditional probabilities
•	Identify examples of applications of Bayes' theorem
## Bayes' formula

Breaking the formula apart

Bayes' theorem is quite intuitive, decomposing the conditional probability of 'A given B' in terms of the probability that both events are true divided by the probability that B is true. Bayes theorem takes this natural idea a step further, expressing the probability that both events are true as a conditional probability multiplied by the condition itself.

To recap:
Bayes' Theorem takes the definition of the conditional likelihood:
 
and rewrites the   as   , which makes perfect sense; the probability of B given A is true, multiplied by the probability that A is true, gives us the probability that both are true.
Making this substitution, you have Bayes' Theorem:
 
## A simple example
Let's take a simple theoretical example to demonstrate. Imagine there are two fish tanks at the local pet store. The small tank holds 10 Betta fish. The large tank has 200 goldfish and 35 Betta fish. Given that a fish is a Betta fish, what's the probability it comes from the small tank?
On the one hand, it seems that if you were to select a fish from the large tank, you'd probably end up with a goldfish. However, because these tanks are of such vastly different sizes, the probability that the fish came from the larger tank is actually more probable.
Using Bayes' theorem, you are looking to find the probability that the fish came from the small tank, given that it is a Betta fish:



# Bayes' Theorem - Lab

## Introduction

In this lab, you'll practice Bayes' Theorem in some simple word problems. 

## Objectives
In this lab you will be able to: 

- Use Bayes' theorem to determine the probability of specific events 

## Define a custom function for Bayes' theorem

To start, write a function, `bayes()`, which takes in the probability of A, the probability of B, and the probability of B given A. From this, the function should then return the conditional probability of A, given that B is true.


```python
def bayes(P_a, P_b, P_b_given_a):
    # Your code here
    return P_a_given_b
```

## Skin Cancer

After a physical exam, a doctor observes a blemish on a client's arm. The doctor is concerned that the blemish could be cancerous, but tells the patient to be calm and that it's probably benign. Of those with skin cancer, 100% have such blemishes. However, 20% of those without skin cancer also have such blemishes. If 15% of the population has skin cancer, what's the probability that this patient has skin cancer? 

> Hint: Be sure to calculate the overall rate of blemishes across the entire population.


```python
# Your code here
```

## Children

A couple has two children, the older of which is a boy. What is the probability that they have two boys?


```python
# Your solution P(2boys|older child is a boy)
```

## A diagnostic test

A diagnostic test is advertised as being 99% accurate 

* If a patient has the disease, they  will test positive 99% of the time 

* If they don't have the disease, they will test negative 99% of the time  

* 1% of all people have this disease 

If a patient tests positive, what is the probability that they actually have the disease?


```python
# Your solution P(Disease | positive test)
```

## Summary 

In this lab, you practiced a few simple examples of Bayesian logic and how you can add prior information to update your beliefs about the chance of events.
