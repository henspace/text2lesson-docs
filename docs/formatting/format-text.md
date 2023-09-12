---
layout: main
---

# Formatting text

_Text2Lesson_ allows you to add some formatting elements to your text. This can be used
to create heading or make some items bold. The format is based on [Markdown](https://daringfireball.net/projects/markdown/),
but there are some limitations. There are also some extensions which are tailored for
use with _Text2Lesson_

# Headings

To create a heading, just start the line with one or more **#** characters,
separated by a space from the heading text. The more hashes, the lower the level.

```
# heading level 1
## heading level 2
### heading level 3
```

becomes

# Heading level 1

## Heading level 2

### Heading level 3

You can also create a level one heading by putting one or more = characters below the line, and a level two heading bu putting one of more - characters
below the line. So:

```
Heading 1
=========

Heading 2
---------
```

becomes

# Heading1

## Heading 2

---

# Italics/emphasis

To put words in italics, just surround them by single underscores. So

> `_this is italic_` becomes _this is italic_.

# Bold

To make words bold, just surround them by double asterisks or underscores. So

> `**this is bold** and __this also__` becomes **this is bold** and **this also**.

# Lists

Simple, single level lists are supported. To start an unordered list, just begin the list item with a \*, + or - character, followed by a space and then the list item.

For an ordered list, just begin the list item with a digit, period, space and then the list item. Here is an example:

```
* item 1
* item 2
* item 3

1. item 1
1. item 1
1. item 1
```

becomes:

- item 1
- item 2
- item 3

1. item 1
1. item 1
1. item 1

# Horizontal lines

Horizontal lines are created by using three or more asterisks or hyphens in a line. Be careful with hyphens as they could turn the preceding line into a heading. You can also add spaces between the characters. The following examples would all create horizontal lines. Noticing how a blank line was left above the three hyphens.

```
***

---
* * *
- - -
```

In conventional Markdown you can also use underscores, but these have special meaning in _Text2Lesson_ to separate problems.
