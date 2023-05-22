---
marp: true
title: DPI 04 CSS
paginate: true
html: true
---

<!-- SOURCE https://firstdraft.slides.com/raghubetina/html-and-css-recap?token=8gU8ghvw -->

# CSS (Cascading Style Sheets)

A **style sheet language** used for describing presentation of a document written in a **markup language**

Created by Håkon Wium Lie at CERN in Switzerland in the 90s so researchers could style documents

---

# CSS Syntax

```css
h1 {
  color: maroon;
  font-weight: 700;
}
```

A **selector**, `h1`

Followed by a **declaration block** within curly brackets `{}`

Each declaration is separated from the next by a semicolon `;`

A **declaration** is comprised of a *property* and a *value* separated by a colon `:`

Collectively, the **selector** and **declaration block** is one **style rule**

---

# Selectors

Selectors are how we specify which HTML elements we want our style rule to apply to.

**Tag Selectors** target all elements of a particular type

e.g. all `<h1>` or all `<ul>`:

```css
h1 {
  color: maroon;
  font-weight: 700;
}
 
ul {
  list-style-type: none;
  padding-left: none;
}
```



---

# Selectors

**Tag Selectors** are usually too broad, so typically we define **Class Selectors** instead by making up a name and preceding it with a dot `.`

```css
.company-name {
  color: maroon;
  font-weight: 700;
}
 
.unstyled-list {
  list-style-type: none;
  padding-left: 0;
}
```

---

# Selectors

We then apply the rules to our HTML elements using the class="" attribute:

```html
	
<h1 class="company-name">Our Awesome Company</h1>
 
<ul class="unstyled-list">
  <li>Our Work</li>
  <li>About Us</li>
  <li>Give Support</li>
</ul>
```

---

# Multiple classes

If possible, it's a good idea to keep your class style rules modular:

```css	
.medium-border {
  border-bottom: 5px grey solid;
}
 
.big-padding {
  padding: 100px;
}
```

---
# Multiple classes

Then, you can combine them by applying multiple classes to the same HTML element:

```html
	
<div class="medium-border big-padding">
  <h1 class="company-name">Our Awesome Company</h1>
 
  <ul class="unstyled-list">
    <li>Our Work</li>
    <li>About Us</li>
    <li>Give Support</li>
  </ul>
</div>
```

---
# Multiple classes

You can still use them individually elsewhere, too, which helps maintain consistency:

```css	
.medium-border {
  border-bottom: 5px grey solid;
}
 
.big-padding {
  padding: 200px;
}
```

```html
<div class="medium-border">
  « Homepage
</div>
 
<p class="big-padding">
  Our mission is to...
</p>
```

---

# CSS Fundamentals

[Open workspace in Replit](https://replit.com/@raghubetina1/CSS-Fundamentals)


---

# External style sheets

Technically you could write CSS right inside an HTML element using the style="" attribute:

```html
<p style="padding: 100px;">Our mission is to...</p>
```

As we've seen, it's much more re-usable to define classes. And even better than putting those classes in a `<style>` element within the same HTML document is to put them in an external style sheet.

Create a file ending in .css and then add a `<link>` element to the HTML file to connect it:

```html
<link rel="stylesheet" href="/my_styles.css">
```

Now you can easily re-use your rules across all the pages in your site.

---

# External style sheets

[Open workspace in Replit](https://replit.com/@raghubetina1/External-style-sheets)

---

# Anything confusing, unclear or fuzzy about CSS?

<iframe src="https://pollev-embeds.com/discourses/sU7vGLU8GeYGy8XwLaGFb/respond" width="1100px" height="600px"></iframe>

---

# Resources

[Mozilla Developer Network MDN](https://developer.mozilla.org/en-US/docs/Web/CSS)

[DevDocs](https://devdocs.io/css/)



