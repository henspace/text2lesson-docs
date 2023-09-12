---
layout: main
---

# Formatting text

_Text2Lesson_ allows you to add some formatting elements to your text. This can be used
to create headings or make some items bold. The format is based on [Markdown](https://daringfireball.net/projects/markdown/),
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

You can also create a level one heading by putting one or more = characters below the line, and a level two heading by putting one or more - characters
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

# Italics and emphasis

To put words in italics, just surround them by single asterisks or underscores. So

```
_this is italic_
*this is italic*
```

becomes

_this is italic_

_this is italic_

# Bold

To make words bold, just surround them by double asterisks or underscores. So

```
**this is bold** and __this is also bold__
```

becomes

**this is bold** and **this is also bold**.

# Lists

Simple, single level lists are supported. To start an unordered list, just begin the list item with an asterisk, plus or minus character, followed by a space and then the list item.

For an ordered list, just begin the list item with any digit followed immediately by a period and space and then the list item. Here is an example:

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

# Links

The basic format for adding links is very simple and just comprises the text you want displayed in square brackets immediately followed by the url or web address in parentheses. So

```
[Visit Text2Lesson](https://text2lesson.com)
```

becomes [Visit Text2Lesson](https://text2lesson.com)

You can add a title which will appear when you hover your mouse over the link. Just follow the url with a space and then the title in double quotation marks, like this:

```
[Visit Text2Lesson](https://text2lesson.com "this is the title")
```

which becomes [Visit Text2Lesson](https://text2lesson.com "this is the title")

Note that the url must begin with http or https; no other protocols are supported.

# Automatic links

As a quicker way of adding links, you can just add the url between less than and greater than characters like this:

```
<https://text2lesson.com>
```

which becomes <https://text2lesson.com>

# Email addresses

In a similar way to creating automatic links, you can add a link to an email address by using the less than and greater than characters. So

```
<fictitious.person@example.com>
```

becomes <fictitious.person@example.com>

# Horizontal lines

Horizontal lines are created by using three or more asterisks or hyphens in a line. Be careful with hyphens as they could turn the preceding line into a heading. You can also add spaces between the characters. The following examples would all create horizontal lines. Notice how a blank line was left above the three hyphens.

```
***

---
* * *
- - -
```

becomes:

---

---

---

---

In conventional Markdown you can also use underscores, but these have special meaning in _Text2Lesson_ and are used to separate problems.

# Blockquotes

To add a blockquote, just precede the line with the greater than (>) character. Nested blockquotes are not supported.

```
> Here is some text as a blockquote
>
> Here is more.
```

becomes

> Here is some text as a blockquote
>
> Here is more.

# Code blocks

To create code blocks, precede each line with four spaces or a tab. The text
will then be presented verbatim with no further processing.

```
    This is line 1 **this won't be bold**
        This is line 2 indented a bit
    This is line 3
```

becomes

    This is line 1 **this won't be bold**
        This is line 2 indented a bit
    This is line 3

# Maths or math if you prefer

_Text2Lesson_ includes some formatting tools to make maths equations simpler. This is a complex topic, so check [Adding maths](add-maths.md) for details.

# Videos

Videos can be embedded in the lesson. See [Adding videos](add-videos.md) for details.
