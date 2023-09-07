---
layout: main
---

# Missing word and order problems

So far we've looked at multiple choice questions and slideshow presentations.
There are two more types of problems of problems that _Text2Lesson_ can handle:

- Missing word problem: in this problem, words are missing from the question, and
  the person playing the lesson has to select the missing word from a number of options.
- Order problem: in this problem, words have to be selected in the correct order.

Let's take a look at how we create these.

# Missing word

This is created by defining a question with what are called missing words. A missing
word is created in the question by typing three dots immediately followed by the missing
word. The question will then be presented with the missing words hidden and replaced
by a set of options from which the correct word must be be selected.

Here is an example:

```
? Complete this sentence:
The playwright ...William ...Shakespeare wrote
Romeo and Juliet.
x John
x Shelley
x Percy
x Keats
```

This question will be shown as:

```
Complete this sentence: The playwright _______ _______ wrote Romeo and Juliet.
```

The wrong answers, created by using the **x** indicator will be added to the
possible options for each word.

Cut and paste that lesson into one of your lesson slots and see what it does.

# Order problem

If the question just has `123` at the end, it creates a ordering problem.

Each of the right answers are put in a row, and they have to be selected in the
same order they were written in the lesson. Any wrong answers are added to the
possible options, to make the question harder. Here is an example:

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

You've now seen how to create all the different problem types. That's the end
of the learning trail.

Take a look at the [Contents](../contents.md) for more advice about getting the
most out of _Text2Lesson_.
