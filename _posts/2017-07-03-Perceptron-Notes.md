---
layout: post
title:  "Perceptron Notes"
date:   2017-07-03 07:00:00 -0600
categories: perceptron, machine learning
permalink: pretty
---

## Short History

Machine learning and artificial intelligence have one significant shared goal that binds them in their conquest to stretch their boundaries, to learn and better understand the human brain.  Before computers were in the hands of humans, **The Perceptron, a Perceiving and Recognzing Automaton** was published in 1957 that discussed an algorithm that would **learn** from data and classify unknown samples provided to it and match it to one class or another.  This Perceptron was modeled off the way we understood neurons.  Neurons was described to be similiar to a simple logic gate with binary outputs.  So information comes in, gets processed, and comes out with a signal.

## Terminology

activiation function - a linear combination of input values,x, and corresponding weight vectors,w, and z is called the net input such that:

$$ z = w_1x_1 + ... + w_mx_m $$
