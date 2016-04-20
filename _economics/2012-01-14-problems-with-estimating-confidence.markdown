---
comments: true
date: 2012-01-14 19:18:24+00:00
layout: post
slug: problems-with-estimating-confidence
title: Problems with Estimating Confidence
wordpress_id: 91
categories:
- Random
---

It's interesting that both business school and law school have insisted that I take a quiz to demonstrate how poorly I gauge confidence. A quantitative analysis and a problem solving course respectively asked a series of questions, such as: "In what year did Gutenberg invent the printing press?" They ask that you to provide your best guess of the answer, and the upper and lower bounds of your 80% confidence interval (i.e. the year for which you are 90% certain it was not invented later and the year for which you are 90% certain it was not invented earlier). When a class is polled, the occurrence of mistakes is usually much greater than the expected 20%. Regarding one such exercise, in which CFOs were asked to estimate stock market returns, [Kahneman](http://en.wikipedia.org/wiki/Daniel_Kahneman) writes in his book _Thinking Fast and Slow_, "[as] frequently happens in such exercises, there were far too many surprises; their incidence was 67%, more than 3 times higher than expected. [This shows gross overconfidence]." Business school, law school, and Kahneman all fail to recognize that this exercise is flawed. Specifically, there are two errors in reasoning.

**1. Failure to recognize that the occurrence of errors says little about the distribution of the guesses**

Suppose we are asked to estimate stock market returns in a given year. We know from historical data that the upper bound of an 80% confidence interval is around 30%. Now suppose that people, on average, are reasonably confident, so that the mean of their upper bound guesses is the upper bound itself (30%). But people's guesses are going to vary. Imagine two superimposed bell curves, one of the stock market returns, and one of people's upper bound guesses. It's far from obvious, but it should be fairly easy to see, after some thought, that if we run this trial multiple times, the occurrence of upper bound errors will be greater than 10%.

To illustrate, take this to the extreme. Suppose 70% of people guess that the upper bound of stock market returns is 70% for a given year, and the other 30% guess the upper bound is -60%. Suppose the chance of both outcomes is zero. Now, we can say that 30% of the population is grossly overconfident, and that 70% is grossly under-confident, but note that the average of their upper bound guesses is 31%, slightly more than 30%. Given these suppositions, the occurrence of upper bound errors will be precisely 30%, three times higher than expected. Can we use this result, as Kahneman did, to say that people were "grossly overconfident"?

In all likelihood Kahneman was right; the CFO's he was talking about probably were, on average, overconfident about their ability to estimate stock market returns. It's just that it's hard to know the extent of their overconfidence, given the difficulty of describing the distribution of their confidence interval estimates from the occurrence of errors.

**2. Failure to recognize that the answer cannot always be treated as a random variable**

Suppose the year in which Gutenberg invented the printing press is normally distributed (joke). Many questions in these exercises ask for arbitrary, not random, numbers. These questions inevitably ask about past data that is already determined. Even if that data was randomly generated in the first place, there are a couple problems with this. [Schrodinger's Cat](http://en.wikipedia.org/wiki/Schr%C3%B6dinger's_cat) illustrates one of them.

Or consider the following question: "I'm thinking of a real number. What's your best guess? State a number such that you're 90% sure that your number is greater than mine." Here creating a confidence interval is impossible. Let's take it a step further: "I'm thinking of a real number between 0 and 1." You might guess 0.9 as the upper bound of your confidence interval. You would be right if the distribution of my real number was uniform, but that's not always the case. There are infinitely many probability distributions I could use to choose my number, and without more information, creating an accurate confidence interval is again impossible.

In the real number example, we are given an upper bound and a lower bound and this information is not enough to form a proper confidence interval. Consider the Gutenberg press question again. My group of five was 100% certain that the printing press did not exist in the 1200s, and 100% certain that it did exist in the 1600s, but as was the case of the random real between 0 and 1, having just this information is not enough to create an accurate confidence interval.

For some questions, it is possible to create a more reasonable confidence interval, but these are a rarity on this sort of exercise. Consider Kahneman's exercise on estimating stock market returns. Here it is possible to create a confidence interval for a given year, even a past year, because we have historical information about the distribution of returns.
