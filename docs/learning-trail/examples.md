---
layout: default
---

# Example lessons

The easiest way to learn _Text2Lesson_ lesson is to look at some examples. All of
these are also included in the _Example quizzes_ book in _Text2Lesson_'s remote
library.

Each quiz introduces a new feature a new feature, so take a look at each one. Play
the lesson in _Text2Lesson_ first, and then take a look at the text that was used
to create the lesson.

# Multiple choice questions

This is the simplest lesson. All it includes is a set of multiple choice questions
with a single answer to each.

1. Play the lesson in the _Text2Lesson_.
1. Take a look at the [Capital cities of Europe](examples/capital_cities_of_Europe.txt) text.

Here is a part of that lesson:

```
? What is the capital of Spain?
= Madrid
x Barcelona
x Seville
x Valencia
```

Hopefully, you can see how easy it is to write the quiz. The text is broken down
into a set of problems or questions by using special indicators.

- **?**: the question mark indicator identifies the question.
- **=**: the equals sign indicator identifies the correct answer.
- **x**: the x indicators identify the wrong answers.

# Multiple choice question with more than one possible answer

Here is another simple lesson. Again, it just comprises a list of questions.
The only difference is that the file has more than one answer starting with an
equals sign. That's because there's more than one possible right anwser.

1. Play the lesson in the _Text2Lesson_.
1. Take a look at the [Famous authors](examples/famous_authors.txt) text.

Again, here is part of that lesson.

```
? Which of these books are by Chaucer?
= The Cantebury tales
= Troilus and Criseyde
x The divine comedy
x Purgatorio
```

# Introductions

Sometimes you will want to give the reader a bit more information about the
question that follows. This is done by adding a introduction item. The introduction
item begins with the character **i**. You can put this in brackets to make it clearer
like this **(i)**. They'll both work.

In this lesson, each question has some introductory.

1. Play the lesson in the _Text2Lesson_.
1. Take a look at the [Animals](examples/animals.txt) text.

And here is an extract showing the introduction:

```
(i) This is a short quiz about animals. Have a go and see how much you know.
? Which of these animals is only found in South America?
= White headed capuchin monkey
x Vervet monkey
x Samango monkey
x Black and white colobus monkey
```

# The learning trail

The next step in the learning trail is to have a look at
[changing an example lesson](changing-an-example-lesson.md).

[Home](../index.md) | [Contents](../contents.md) | [About](../about.md) | [Privacy](../privacy.md)
