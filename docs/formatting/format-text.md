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

# Font size

You can also increase the font size of text by enclosing it between two size tags like this:

```
{big}This is {big}very big{big} text.
```

becomes

This is <span style="font-size:130%">very big</span> text.

The following size tags are recognised: **big**, **bigger**, **biggest**, **massive**, and **giant**.

# Superscript and subscript

_Text2Lesson_ does not normally allow you to include HTML in your lessons. There
are however a few exceptions. Superscript and subscripts tags are a couple of exceptions.

```
here is<sup>superscript</sup> and here is<sub>subscript</sub>
```

becomes

here is<sup>superscript</sup> and here is<sub>subscript</sub>

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

## Limitation

Standard [Markdown](https://daringfireball.net/projects/markdown/) allows complex block
elements to be included in lists; _Text2Lesson_ does not! Only simple lists are supported: blockquotes, code blocks and other block elements cannot be included.

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

## Limitation

Standard [Markdown](https://daringfireball.net/projects/markdown/) allows reference links to be created; _Text2Lesson_ does not!

# Automatic links

As a quicker way of adding links, you can just add the url between less than and greater than characters like this:

```
<https://text2lesson.com>
```

which becomes <https://text2lesson.com>

## Deviation from standard Markdown

Automatic links in standard [Markdown](https://daringfireball.net/projects/markdown/) are created by enclosing the link between `<` and
`>` characters. As a byproduct of the fact that, unlike Markdown,
_Text2Lesson_ escapes most HTML, if you were to enclose text between `&lt;` and
`>` text, that would also be interpreted as an automatic link. You can prevent
this by using `&gt;` for the closing greater than character. This behaviour is
summarised below:

- `<https://henspace.com>` creates an automatic link.
- `&lt;https://henspace.com>` also creates an automatic link.
- `&lt;https://henspace.com&gt;` does not create an automatic link.

# Email addresses

In a similar way to creating automatic links, you can add a link to an email address by using the less than and greater than characters. So

```
<fictitious.person@example.com>
```

becomes <fictitious.person@example.com>

# Paragraphs

Even though you might write your text on separate lines, _Text2Lesson_ normally
joins lines together. If you want text to appear as a new paragraph, you should include
a blank line.

```
This line will
join with the next.

But this is separate because
of the blank line above.
```

becomes

> This line will
> join with the next.
>
> But this is separate because
> of the blank line above.

_Text2Lesson_ does not normally allow you to include HTML in your lessons. However,
**<br>** is an exception. You can use it to force a new line.

```
This line<br>breaks.
```

becomes

> This line<br>
> breaks

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

## Limitation

Standard [Markdown](https://daringfireball.net/projects/markdown/) allows nested
blockquotes: _Text2Lesson_ does not!

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

_Text2Lesson_ includes some formatting tools to make maths equations simpler. This is a complex topic, so check out [Adding maths](add-maths.md) for details.

# Embedding HTML

_Text2Lesson_ does not normally allow HTML to be included in text; however, there are some exceptions.

- `<br>`: line breaks
- `<sup></sup><sub></sub>`: subscript and superscript
- `&mdash;`: all HTML entities
- attributions: attribution code generated by [Wikimedia Commons](https://commons.wikimedia.org/wiki/Main_Page) can be embedded. See [Using Wikimedia Commons](./using-wikimedia-commons.md).
- MathML: [MathML](https://developer.mozilla.org/en-US/docs/Web/MathML) code can be
  embedded. See [Using MathML](./maths-ml.md).
