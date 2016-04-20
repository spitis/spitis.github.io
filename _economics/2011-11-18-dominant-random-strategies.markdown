---
comments: true
date: 2011-11-18 22:55:29+00:00
layout: post
slug: dominant-random-strategies
title: 'Dominant Random Strategies: Why Judges Are Sometimes Better Off Flipping Coins'
wordpress_id: 8
categories:
- Random
---

**In cases in which policy arguments for a choice can go both ways, judges, agencies, and other decision makers are sometimes better off flipping a coin than making an arbitrary, or even qualified choice. **

There is a big debate over what methods judges should use to interpret written laws. The choice of interpretation often has grave consequences. In one case, a man's prison sentence depended on the interpretation of "using" a gun. If "use" referred only to shooting a gun, he was innocent, but if it also included trading a gun for drugs, he would be guilty (see [Smith v. US](http://en.wikipedia.org/wiki/Smith_v._United_States)). The problem here is not the result of the case - the "justness" or "correctness" of the result is largely ignored in the decision; rather, the problem is that the Supreme Court, in this case among _many_ others, fiercely debates the correct _method_ of interpretation.

Without stating what they are, we can assume that the choice of method has policy implications - there are simply too many smart people debating the issue for it to be a moot point. It's not very clear that courts apply any sort of consistent approach, though the debate seems to suggest that there should be one. Since there is a divide, and (apparently) consistency does not matter much, perhaps choosing which method to use when interpreting laws is a decision best made by flipping a coin.

**Math that inspires the result:**

Here's [a neat math puzzle](http://blog.xkcd.com/2010/02/09/math-puzzle/). Solve it now if you're up to the challenge, or read on for a big hint.

What makes this problem interesting is that the when Alice picks the "two different real numbers by an unknown process", she is picking them arbitrarily, not at random. It turns out that this makes a difference to our strategy, and this particular puzzle is a complex demonstration of the idea that arbitrary is not the same as random.

Let's simplify things:

Suppose Alice picks a secret number from one to six inclusive, and you win $1 if you guess it correctly. It makes a difference if Alice chose her number arbitrarily or if she rolled a hidden die. Do you see why?

If Alice rolls a dice, we can simply guess "1" and be guaranteed a one in six chance of guessing correctly. But if Alice instead just chose 6 every time she played this game, we would be guaranteed a loss if we guess "1". We can eliminate this uncertainty by using a random strategy. If we roll a dice instead of just calling our an arbitrary number, we can guarantee ourselves a one in six chance of guessing correctly regardless of how Alice chooses her number.

All this talk of random strategies should give you a huge hint as to how to solve the math puzzle. Whereas in the simple example above, a random strategy simply guaranteed a one in six chance of winning, a random strategy in the math puzzle actually produces a greater than 50% chance of winning. Here is the [solution](http://blog.xkcd.com/2010/02/09/math-puzzle/comment-page-1/) (the first comment). An intuitive geometric solution exists, but it's hard to explain over the Internet, so if the algebra doesn't convince you... take my word for it - the solution works.

**How it applies to law:**

For decisions in which consistency does not matter, it follows from the above discussion that when offered a choice between two mutually exclusive judicial strategies, with equal policy arguments on both sides, we are better off flipping a coin. Notice that the "correct" strategy - that is, the one that best advances policy objectives - is an _unknown known_. Although we don't know which strategy is better, one is necessarily better. This is analogous to Alice picking a number of her choice instead of rolling a dice. We don't know what that number is, but it's necessarily one of the six choices. Therefore, if we pick one strategy and stick with it, we risk being wrong 100% of the time (of course, we could also be right 100% of the time). If we instead flip a coin and choose our strategy at random, we are guaranteed the correct strategy 50% of the time. In some cases, if the consistency of methodology does not matter, this is the dominant strategy.

Interestingly, a 50/50 coin flipping strategy may be superior even in cases in which we think that policy arguments lean towards one side. This occurs because of society's natural risk aversion (more on this later - for now assume that society uses the natural logarithm as its utility function). Here is a quantitative demonstration (please excuse my outlandish numbers, and the several implicit assumptions I'm making here - an extreme example is sufficient and within my mathematical capability; also note the most important assumption is that the costs and benefits don't compound):

Suppose policy considerations give us 60% confidence that Strategy A is the correct strategy, and that using the correct strategy keeps the status quo, but using the incorrect one costs a relevant administrative agency $1 each decision. Suppose there are two such decisions a year, and that the relevant agency has an annual budget of $3.

The Expected Utility of using Strategy A for both decisions is

$$0.4\cdot \ln (\frac{1}{3}) + 0.6\cdot \ln (1) = -1.1$$

whereas the utility of flipping a coin is

$$0.25\cdot \ln (\frac{1}{3}) + 0.5\cdot \ln (\frac{2}{3}) + 0.25\cdot \ln (1) = -.58.$$


In this example, sticking to a single strategy is nearly twice as bad as flipping a coin, even though we were 60% sure that the single strategy we chose was correct. This suggests that flipping a weighted coin might be better than both options.

Intuitively, the result occurs because we prefer moderate outcomes to extreme outcomes. You can see how this result might extend to more reasonable scenarios (smaller relative costs each decision, but more decisions / year).

So, going back to the legal starting point, we see that if a judge (or agency?) is faced with a decision between two methodologies that arrive at different results, and there is no consistency reason for him to pick one or the other, he might be better off flipping a coin.
