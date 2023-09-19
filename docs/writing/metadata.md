---
layout: main
---

# Metadata

Metadata serves two main purposes:

- it allows you to provide details about who wrote the lesson, copyright information and how it is licensed.
- it also allows you to provide additional information about the lesson that can be included later in your problems. This allows you to give some text a label, and then repeat that text later in your lesson by using the label.

# Defining metadata

Metadata is defined by adding additional information at the beginning of the
lesson file before the first problem is defined.

All lines at the start of the lesson preceding the first problem are regarded as
potential metadata.

The format of a metadata definition is a line starting with a `key` followed by
its value. The key cannot have any spaces in its name and can only comprise the
characters a to z, A to Z, 0 to 9, and the underscore.

`Key: the value`

The key must be separated from its value by a colon, semi-colon, or period. Any
of these can be immediately followed by a hyphen if preferred. There can be any
number of spaces surrounding the key, separator and values. Keywords are
converted to uppercase, so _mykey_, _MYKEY_ and _MyKey_ will be treated as the
same key.

Here are some examples of valid keys:

```
AUTHOR: John Doe
mykey:- some text
```

If a definition is repeated, it overwrites any previous value. Any other lines
that preceding and which are not identified as metadata are ignored. This allows
you to add your own comments to the start of the lesson by just starting the line
with any invalid key character such as `@` or `#`.

You can create your own keys, but some are reserved and are used for [author and licensing information](#author-and-licensing-information).

Here is an example of the start of a valid lesson file:

```
# this is just a comment and is ignored.
AUTHOR: John Doe
MyKey: some text to use later
AnotherKey   :  more text but note the use of spaces.

(i) Here is the first problem which prevents any further definitions.
```

# Using metadata

Metadata can be incorporated into your lessons by utilising the `meta:key` text.

Look at this lesson file:

```
MyName: John

(i) Welcome to this lesson written by meta:MyName.
```

The lesson starts by creating metadata using the key `MyName`. Then the
introduction uses the key with the text `meta:MyName`. The resulting introduction
is shown below:

```
Welcome to this lesson written by John.
```

Notice how `meta:MyName` has been replaced by the metadata's value of `John`.

# Limitations

Metadata can only be used for simple replacements. You cannot include any
[formatting](../formatting/format-text.md) in the metadata values.

# Author and licensing information

The following metadata keys have special meaning within _Text2Lesson_:

- **TITLE**: the lesson title
- **AUTHOR**: the lesson's author
- **COPYRIGHT**: the copyright for the lesson
- **LICENSE**: the license under which the lesson in released. LICENCE is also accepted.
- **ATTRIBUTION**: any additional attribution that is required. This may be appropriate if you are modifying a lesson that had been released under a Creative Commons by Attribution license.

If either the **AUTHOR** or **COPYRIGHT** keys are set, these values, along with the **LICENSE** and **ATTRIBUTION** values, are used to provide additional information on the certificate at the end of the lesson.

The following license names are recognised and will be automatically converted to a link:

- **CC0**: [CC0 1.0 Universal Public Domain Dedication](https://creativecommons.org/publicdomain/zero/1.0/)
- **CC BY-xx**: [Creative Commons licences](https://creativecommons.org/licenses/). CC BY-SA, CC BY-NC, CC BY-NC-SA, CC BY-NC-ND licences are recognised. They can be followed by a version, e.g `CC BY-SA 2.5`. The version defaults to 4.0 if omitted.
