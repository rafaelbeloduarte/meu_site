+++
draft = false
date = 2022-08-18T15:21:04-03:00
title="The Monty Hall Problem"
description=""
slug="monty-hall-problem"
tags = ["statistics", "probability"]
categories = []
externalLink=""
series = []
author = "Rafael"
+++

The book "The Drunkards Walk" [^fn1] deals with how randomness influences our lives and the difficulties people have in understanding probability.

In one of the passages, to illustrate this last point, the author brings up the following problem:

Imagine that you are given a choice between 3 doors, behind one of the doors there is a prize and the others hide a goat.

After you have made the choice, one of the doors where there is nothing is opened and you are given the choice to change the door or not.

What's more advantageous? To swap or not? Or does it not make a difference?

My first instinct, like that of most people according to the author, is that it doesn't matter if I swap doors or not, there are only two doors and the probability of winning is 1/2.

But that is not true, the probability of winning if I swap doors is 2/3! Whereas if I don't, I continue with the initial winning probability of 1/3.

# Why?

Because when one of the doors was revealed to me, I had additional information and the space of possibilities changed. Before, one had the random choice between the 3 doors, now it's the choice between swapping doors or not. Those are two DIFFERENT choices.

The second choice can be made by answering the following question: what is the probability of choosing the wrong door? It's 2/3. Thus, 2/3 of the times the wrong door will be chosen and in those times it will be advantageous to switch.

We can experiment with the problem using the following algorithm:

1. Generate a random list, say `0` are the empty doors and `1` the prize;
1. Choose a door (an index of the list) at random;
1. Remove one of the empty doors (any `0`);
1. Swap doors;
1. Repeat `n` times, adding the `result` of our choice to the previous ones;
1. Divide the sum by `n`.

This will give us the ratio of successes. In `python` one can write the code below. Iterating 1 million times, the ratio is very close to 2/3: 0.667355.

```python
import random

n = 1000000
result = 0

for i in range(1, n):
     list = [0,0,1]
     # shuffle the list
     random.shuffle(list)
    
     # choose a door
     choice = random.choice(list)
    
     # remove 1 zero (door with no prize)
     list.remove(0)
     # swap doors
     index = list.index(choice)
     if index == 0:
         index = 1
     else: index = 0
    
     # save the result
     result = result + list[index]

# calculate the ratio of successes
prop = result/n
print("########################")
print("")
print("Success ratio = ", prop)
print("")
print("########################")
```

## References

[^fn1]: Mlodinow, Leonard, 1954-. The Drunkard's Walk: How Randomness Rules Our Lives. New York: Pantheon Books, 2008.
