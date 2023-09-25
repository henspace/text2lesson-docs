---
layout: main
---

# 📄 Example lessons

The easiest way to learn _RapidQandA_ is to look at some examples. All of
these are also included in the _Example quizzes_ book in _RapidQandA_'s remote
library.

Each quiz introduces a new feature, so take a look at each one. Play
the lesson in _RapidQandA_ first, and then take a look at the text that was used
to create the lesson.

# Capital cities of Europe: multiple choice questions

This is the simplest lesson. All it includes is a set of multiple choice questions
with a single answer to each.

1. Play the lesson in _RapidQandA_.
1. Take a look at the [Capital cities of Europe](examples/capital_cities_of_Europe.txt) text.

Here is a part of that lesson:

```
(?) What is the capital of Spain?
= Madrid
x Barcelona
x Seville
x Valencia
```

Hopefully, you can see how easy it is to write the quiz. The text is broken down
into a set of problems or questions by using special indicators.

- **(?)**: the question mark indicator identifies the question.
- **=**: the equals sign indicator identifies the correct answer.
- **x**: the x indicators identify the wrong answers.

The parentheses around the question mark are optional, but they normally make it
easier to identify the question.

> <span style="font-style: normal; font-size:2em;">⚠️</span> Make sure you have a space or right-hand bracket after the indicator, otherwise it won't be recognised as such.

# Famous authors: multiple choice question with more than one possible answer

Here is another simple lesson. Again, it just comprises a number of questions.
The only difference is that the questions have more than one answer starting with an
equals sign. That's because there's more than one possible right answer.

1. Play the lesson in _RapidQandA_.
1. Take a look at the [Famous authors](examples/famous_authors.txt) text.

Again, here is part of that lesson.

```
(?) Which of these books are by Chaucer?
= The Canterbury tales
= Troilus and Criseyde
x The divine comedy
x Purgatorio
```

# Animals: introductions

Sometimes you will want to give the reader a bit more information about the
question that follows. This is done by adding a introduction item. The introduction
item begins with the character **i**. Again, you can put this in parentheses to make it clearer
like this **(i)**. They'll both work.

In this lesson, each question has some introductory text.

1. Play the lesson in _RapidQandA_.
1. Take a look at the [Animals](examples/animals.txt) text.

Here is an extract showing the introduction:

```
(i) This is a short quiz about animals. Have a go and see how much you know.
(?) Which of these animals is only found in South America?
= White headed capuchin monkey
x Vervet monkey
x Samango monkey
x Black and white colobus monkey
```

# The learning trail

The next step in the learning trail is to have a look at
[changing an example lesson](changing-an-example-lesson.md).
