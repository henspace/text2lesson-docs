---
layout: main
---

# Slideshows

Previously we looked at adding a introduction to a lesson by using the **(i)** indicator.

Here is an example lesson with an introduction.

```
(i) This is a short quiz about animals. Have a go and
see how much you know.
(?) Which of these animals is only found in South America
= White headed capuchin monkey
x Vervet monkey
x Samango monkey
x Black and white colobus monkey
```

The introduction pops up just before the question. That's the standard way
to add introductions for each problem. Those indicators, **(i)**, **(?)**, **=**, and **x** are
all used to define a problem, and our lesson can contain as many problems as we
want.

But what if we create an introduction with no associated question? Here is an example:

```
(i) Here is some introductory text.

It's made up of multiple paragraphs.

But it has no associated question.

(i) This is a short quiz about animals. Have a go and see how much you know.
(?) Which of these animals is only found in South America?
= White headed capuchin monkey
x Vervet monkey
x Samango monkey
x Black and white colobus monkey
```

In the example above, we have two **(i)** indicators. Whenever _Text2Lesson_ sees
a new introduction indicator, it knows it is the start of a new problem. So here
we have defined two problems:

1. The first just has an introduction talking about paragraphs, but no question.
1. The second has its own introduction and a question about monkeys.

So what does _Text2Lesson_ do?

Because the first introduction has no question, it becomes a slideshow.

You saw how to edit a lesson in [changing an example lesson](changing-an-example-lesson.md),
so now try adding an introduction to the lesson, but with no associated question.
If you want, you can copy and paste the text below into the lesson and see what it does.

```
(i) Turning and turning in the widening gyre

The falcon cannot hear the falconer;

Things fall apart; the centre cannot hold;

Mere anarchy is loosed upon the world,

(i) Today's topic is poetry.
(?) You've just read a short extract from a famous poem
called "The Second Coming". But who wrote it?
= William Butler Yeats
x William Wordsworth
x John Keats
x Ralph Waldo Emerson
```

# The learning trail

The next step is to look at the last two types of problem: [missing word and order problems](missing-word-and-order.md).
