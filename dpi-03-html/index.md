---
marp: true
title: DPI 03 HTML CSS
paginate: true
html: true
---

<!-- SOURCE https://firstdraft.slides.com/raghubetina/html-and-css-recap?token=8gU8ghvw -->

# HTML (HyperText Markup Language)
* A **markup language** that **web browsers** use to display text, links, images and other media
* Created by Tim Berners-Lee at CERN in Switzerland in the early 90s so researchers could create and share documents

---

# HTML Syntax

```html
<a href="https://www.wikipedia.org">
  Go to Wikipedia
</a>
```

* Opening tag `<a>`
* Closing tag, `</a>`
* Content in between, `Go to Wikipedia`
* Attributes inside the opening tag, `href=""`
* Collectively, we call this an **element**
---
# HTML Syntax

```
<a href="https://www.wikipedia.org" target="_blank">
  <img src="/wikipedia.jpg" alt="Go to Wikipedia">
</a>
```

* Elements can have more than one **attribute**.
* Elements can contain other elements.
  * In that case, the one inside is known as a **child element** and the one outside is the **parent element**.
  * If there are multiple levels of **nesting**, then all the elements inside an outer element are its **descendants**.

---
# Attributes
* Most attributes only make sense on specific elements.
  * `href=""` is for `<a>` elements, to specify where to take the user when they click the link.
  * `src=""` is for `<img>` elements, to specify the url of the image to load.
  * `for=""` is for `<label>` elements, to specify which input element it is paired with.
* Some attributes can be put on almost any element, like `class=""` or `id=""`.
* ​Any **id** should only be used once per document.
* A **class** can and should be used repeatedly.

---

# Boilerplate

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- where we tell the browser how to process the document: -->
        <!-- what title to put in the browser tab -->
        <!-- what style sheets to load -->
        <!-- what language to use -->
          <!-- we will always use a character set called UTF-8 -->
          <!-- UTF-8 allows for all languages as well as things like emoji -->
  </head>
  <body>
    <!-- content displayed to user -->
  </body>
</html>
```

---
# Replit

* You'll need to sign up for a [Replit](https://replit.com/) account, a cloud-based code editing environment
* You can sign in with your GitHub account if you want.
* Click the blue "Fork REPL" button in the top-right corner to get a workspace to play around in.
* Read the code, modify the code, play around and make sure that you understand every single line. Ask any questions that occur to you.

---

# Basic HTML Content

[Open Replit Workspace](https://replit.com/@raghubetina1/Basic-content)

---
# HTML Lists

[Open Replit Workspace](https://replit.com/@raghubetina1/Lists)

---
# Forms
* There's one more essential element `<form>`.
* We can't really do anything with forms right now, since HTML can't process input — it's a formatting language.
* We'll learn about forms after we learn enough Ruby and Ruby on Rails to do things with user input.

---

# Anything confusing, unclear or fuzzy about HTML?
<iframe src="https://pollev-embeds.com/discourses/T2RZWoljaNo5qvN5ZNUTG/respond" width="1100px" height="600px"></iframe>

---

# Resources

[Mozilla Developer Network, MDN](https://developer.mozilla.org/en-US/)

