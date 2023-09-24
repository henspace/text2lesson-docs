---
layout: main
---

# 😰 Troubleshooting

Hopefully, you'll find creating lessons straightforward and won't need to visit this page often. Sometimes, however, you might find things don't behave quite the way you expect. Below are some issues you might experience.

# Why doesn't my lesson show up as a slideshow?

So you created some information that you want to appear as a slideshow. Unfortunately,
it just appears as a static dialog box preceding the next question. What's wrong?

If _RapidQandA_ finds an introduction followed by a question, it assumes the
introduction is part of the question and so shows it in the dialog box. To tell
_RapidQandA_ that this is a separate problem and should be shown separately as
a slide show, you need to use the separator indicator.

This example will treat the information `(i)` as part of the question `(?)` that
follows. It **will not** appear as a slideshow.

```
(i) This is my slideshow.

Here is another slide.

(?) Here is the question. Did the information appear as a slideshow?
= yes
x no
```

However, in this example, we've added the separator `_____`. Now, _RapidQandA_ will treat the information `(i)` as a separate problem and it **will** appear as a slideshow.

```
(i) This is my slideshow.

Here is another slide.
_____
(?) Here is the question. Did the information appear as a slideshow?
= yes
x no
```

# It keeps telling me I haven't added any answers, but I have.

You must have a space or right bracket after the `=` and `x` indicators.

This will be detected as a right answer:

```
= London
```

This won't:

```
=London
```

# One of my questions is missing

This can happen if you forget to add an **i** or **?** indicator after a \***\*\_\*\*** separator.

Imagine you type this:

```
_____
What is the capital of the UK?
= London
x Paris

(?) What is the capital of France?
= Paris
x London
```

When _RapidQandA_ runs, it will see the separator and then look for the next introduction **i** or question **?** indicator. It will ignore everything else. In this example the first question it will find will be `What is the capital of France?` It will ignore the one about the capital of the UK as it wasn't flagged as a question.

> <span style="font-size:2em;">⚠️</span> Make sure you don't forget your introduction or question indicators.

This is what the lesson should have looked like:

```
_____
(?) What is the capital of the UK?
= London
x Paris

(?) What is the capital of France?
= Paris
x London
```

# It keeps crashing or won't start up

Whoops! Sorry about that. It's possible the memory has become corrupt. _RapidQandA_
should be able to recover, but perhaps something's been missed &mdash; blame the
programmer.

You can clear all the memory to start afresh. Check
[delete everything forever](./deletion-tool.md) for details on how to do this.
