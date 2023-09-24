---
layout: main
---

# 🕵️ Missing word and order problems

So far we've looked at multiple choice questions and slideshow presentations.
There are two more types of problems that _RapidQandA_ can handle:

- **Missing word problem**: in this problem, words are missing from the question, and
  the person playing the lesson has to select the missing word from a number of options.
- **Order problem**: in this problem, words have to be selected in the correct order.

Let's take a look at how we create these.

# Missing word problem

This is created by defining a question with what are called missing words. A missing
word is created in the question by typing three dots immediately followed by the missing
word.

The question is presented with the missing words hidden and replaced
by fields from which the correct answer can be selected. The possible answers are
presented as a drop-down list of options formed from all the missing words combined with
any wrong answers that were defined.

Here is an example:

```
(?) Complete this sentence:
The playwright ...William ...Shakespeare wrote
Romeo and Juliet.
x John
x Shelley
x Percy
x Keats
```

This question would be shown as:

```
Complete this sentence: The playwright _______ _______ wrote Romeo and Juliet.
```

The wrong answers, created by using the **x** indicator are added to the
possible options for each word.

Cut and paste the above lesson into one of your lesson slots and see what it does.

# Order problem

If the question just has `123` at the end, it creates a ordering problem.

At the end of the question, a row of fields are added &mdash; one for each of the defined right answers.

The possible answers for each field are presented as a drop-down list of options formed from all the right answers combined with any wrong answers that were also defined.

The correct answer for each field are taken as being in the same order as the right answers
were defined. Here is an example:

```
? Put the prime numbers in ascending order. 123
= 19
= 23
= 29
x 21
x 25
x 27
```

This will make more sense when you try it, so copy the text into a lesson, and
see how it plays.

By default, the options are laid out in a row. Sometimes you might want them
laid out in a column. You can define the orientation by following `123` with the
`>` character followed by the orientation you want.

- Arrange in a row:
  - 123
  - 123>row
  - 123>line
- Arrange in a column:
  - 123>col
  - 123>column

# The learning trail

You've now seen how to create all the different problem types. Let's look at how
we can craft a problem using those five different types in [One problem, five ways](./one-problem-five-ways.md).
