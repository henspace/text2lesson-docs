---
layout: main
---

# Using Wikimedia Commons

[Wikimedia Commons](https://commons.wikimedia.org/wiki/Main_Page) is a fantastic
resource for free images. Because it is such a good source, _Text2Lesson_ provides
special support for images you might find there. Follow these simple steps to use
an image from [Wikimedia Commons](https://commons.wikimedia.org/wiki/Main_Page)
in _Text2Lesson_.

1. Go to [Wikimedia Commons](https://commons.wikimedia.org/wiki/Main_Page).
1. Use the search tools to find the image you want.
1. When you find the image, select **More Details**.
1. Find the the **Use this file on the web** link. If you're on a mobile and the
   link isn't available, scroll to the bottom of the page and select **Desktop**.
1. When you click on the link, a **Use this file on the web** dialog box will pop up.
1. Copy all the text from the **Embed this file** field to the clipboard. The **HTML**
   option should be selected.
1. Paste the text into your lesson file.
1. _Text2Lesson_ will automatically extract the image and attribution details; you
   don't need to do anything.
1. An example is shown below:

> `<a title="Martin Vorel, CC BY-SA 4.0 &lt;https://creativecommons.org/licenses/by-sa/4.0&gt;, via Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File:Programming_code.jpg"><img width="512" alt="Programming code" src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ef/Programming_code.jpg/512px-Programming_code.jpg"></a>`

## Image alignment

In the [Adding Images](add-images.md) topic, you will have seen how to push an
image to the left by adding the **<** character. You can do a similar thing with
the embedded code from [Wikimedia Commons](https://commons.wikimedia.org/wiki/Main_Page).
Just prefix the code with another **<** character. So the following text would push
the image to the left.

> `<<a title="Martin Vorel, CC BY-SA 4.0 &lt;https://creativecommons.org/licenses/by-sa/4.0&gt;, via Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File:Programming_code.jpg"><img width="512" alt="Programming code" src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ef/Programming_code.jpg/512px-Programming_code.jpg"></a>`

Notice that it starts with `<<a` and not `<a`.

# Using Wikimedia Commons for your own images.

[Wikimedia Commons](https://commons.wikimedia.org/wiki/Main_Page) also allows
you to upload your own images and then embed them in web pages. This makes it ideal
for use with _Text2Lesson_.

Images you add should really be for educational purposes, but that of course fits
nicely within the aim of _Text2Lesson_. You also need to make any content
you create [free content](https://en.wikipedia.org/wiki/Free_content), normally under
a [Creative Commons licence](https://en.wikipedia.org/wiki/Creative_Commons_license).
That again fits in with the ethos of _Text2Lesson_.
