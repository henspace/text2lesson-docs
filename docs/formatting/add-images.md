---
layout: main
---

# 🖼️ Adding images

> <span style="font-size:2em;">💡</span> Tip: [Using Wikimedia Commons](./using-wikimedia-commons.md) is the easiest and recommended way for adding images to _RapidQandA_.

In any text based programs, adding images can always be a bit of a problem. Let's
see how it's done in _RapidQandA_. The basic format is very simple:

```
![alternative text](url-of-the-image)
```

- The **alternative text**, or alt-text, is a description of the image, which is displayed if your image can't
  be displayed for any reason. It's also important for readers with any visual
  impairment, as this text may be spoken by screen readers.
- The **url-of-the-image** is the url (web address) of the image.

So here is the text that can be used to show the _RapidQandA_ logo.

```
![Small logo showing T2L following by bulleted lines](https://henspace.github.io/text2lesson-docs/assets/images/logo/bordered_logo_128.png)
```

You can also add a title which will appear when you hover over the image. You do
that by following the url with a space and then the title in double quotes. So
a full image definition would look like this:

```
![alternative text](url-of-the-image "title of image")
```

Now you may have realised an issue: where are the images stored? They have to be
available online to use them in _RapidQandA_. Because _RapidQandA_ is inherently
intended for educational purposes, the ideal place to get or store your images is
[Wikimedia Commons](https://commons.wikimedia.org/wiki/Main_Page). _RapidQandA_ has some specific features to make dealing with images
from [Wikimedia Commons](https://commons.wikimedia.org/wiki/Main_Page) even easier. Check out [Using Wikimedia Commons](using-wikimedia-commons.md)
for more details.

# Image alignment

Images are normally positioned automatically. However, you can ask the application to push the image to
the left of the page. You do this by adding **<**, which sort of points to the left, between the starting **!** and **[** characters. So this line would push the image to the left:

```
!<[alternative text](url-of-the-image "title of image")
```

# Attributions

If you use any images in your lessons, you obviously need to make sure you have
permission to use and distribute the images. You will often find that for
free images, you need to provide attribution. _RapidQandA_ allows you to add
attribution details to the title. Note that _RapidQandA_ can produce the attributions
automatically for images if you [use Wikimedia Commons](using-wikimedia-commons.md).

The extended title contains a number of elements
separated by the **|** character. The full format is as follows:

```
"title|original-source-url|authors|licence-name|licence-url|notes"
```

- **title**: the title of the image.
- **original-source-url**: this where you originally obtained the image and is normally different from the url used to display the image.
- **authors**: these are the names of the people who created the image. In most cases it will be a single name.
- **licence-name**: this is the short name of the licence. For example `CC BY-SA` or `PUBLIC DOMAIN`.
- **licence-url**: this is the url for the details of the licence. If you omit this, the application will try to determine it from the licence-name. The following licence names are recognised:
  - **CC0**: [CC0 1.0 Universal Public Domain Dedication](https://creativecommons.org/publicdomain/zero/1.0/)
  - **CC BY-xx**: [Creative Commons licences](https://creativecommons.org/licenses/). CC BY-SA, CC BY-NC, CC BY-NC-SA, CC BY-NC-ND licences are recognised. They can be followed by a version, e.g `CC BY-SA 2.5`. The version defaults to 4.0 if omitted.
  - **Unsplash**: [Unsplash licence](https://unsplash.com/license) for free photos from [Unsplash](https://unsplash.com).
- **notes**: this part contains extra information. For example, if you cropped the image, you might want to add `image cropped`.

If you want to miss out any parts, still leave the **\|** characters in place.

Here are some example titles (note: these are just the titles and not the full image references):

- `Photo of vase|https://henspace.com/fictitious-image.png|John Doe|CC BY 4.0|https://creativecommons.org/licenses/by/4.0/|made monochrome`
- `Photo of car|https://henspace.com/fictitious-image.png|John Doe|Public Domain||`

Attributions are automatically made available on the question pages, and on printed sheets.
