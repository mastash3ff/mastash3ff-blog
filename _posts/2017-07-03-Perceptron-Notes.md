---
layout: post
title:  "Perceptron Notes"
date:   2017-07-03 07:00:00 -0600
categories: perceptron, machine learning
permalink: /perceptron_notes/
---

## Short History

Machine learning and artificial intelligence have one significant shared goal that binds them in their conquest to stretch their boundaries, to learn and better understand the human brain.  Before computers were in the hands of humans, **The Perceptron, a Perceiving and Recognzing Automaton** was published in 1957 that discussed an algorithm that would **learn** from data and classify unknown samples provided to it and match it to one class or another.  This Perceptron was modeled off the way we understood neurons.  Neurons was described to be similiar to a simple logic gate with binary outputs.  So information comes in, gets processed, and comes out with a signal.

## Terminology

Activation Function - a linear combination of input values(x), corresponding weight vectors(w), which equals the net input(z) such that $$ z = w_1x_1 + ... + w_mx_m $$

Learning Rate - a constant between 0.0 and 1.0 that controls how dramatic the weights are updated.

Epochs - Number of passes over a training dataset

Vectorization - An elemental arithmetic operation is automatically applied to all elements in an array.

OvA(One-vs-All) - A technique used to extend a binary classifier to multi-class problems where the particular class is treated as the positive class and the samples from all other classes are considered as the negative class.

Quantizer - similiar to a unit step function

## Quick Rundown of Algorithm

- Simple and intuitive learning algorithm
- Requires that two classes of data are linearly seperable
- Dependent on learning rate to be small enough



