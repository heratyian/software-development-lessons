# CSS
This lesson goes over CSS: why and how we use it

<!-- TODO -->
## [Slides](../slides/css/index)

## Topics
- CSS

## Story
- Olivia, a talented artist, wants to showcase her artwork on the web. 👩‍🎨
- She discovered **CSS**, the magical language for styling web pages. ✨💻
- CSS allowed Olivia to bring her designs to life and create visually captivating experiences.
- She used CSS to customize colors, fonts, layouts, and more on her web pages. 🎨🎉
- The power of cascading in CSS allowed changes to ripple through multiple **elements**. 🌊💫
- Olivia used CSS selectors to **target** specific **elements** and apply **styles**.
- She explored advanced CSS features like media queries, animations, and transitions. 📐🎥
- CSS became Olivia's artistic palette, and the web became her canvas. 🎨🌐
- With CSS, Olivia's artwork leaped off the screen, captivating her audience.
- CSS turned Olivia's designs into breathtaking masterpieces on the web. 🎭✨

## CSS (Cascading Style Sheets)
- A **style sheet language** used for describing presentation of a document written in a **markup language**

### CSS Syntax

```css
h1 {
  color: maroon;
  font-weight: 700;
}
```

- A **selector**, `h1`
- Followed by a **declaration block** within curly brackets `{}`
- Each declaration is separated from the next by a semicolon `;`
- A **declaration** is comprised of a *property* and a *value* separated by a colon `:`
- Collectively, the **selector** and **declaration block** is one **style rule**

### Selectors
- Selectors are how we specify which HTML elements we want our style rule to apply to.
- **Tag Selectors** target all elements of a particular type
- e.g. all `<h1>` or all `<ul>`:

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

- **Tag Selectors** are usually too broad, so typically we define **Class Selectors** instead by making up a name and preceding it with a dot `.`

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

- We then apply the rules to our HTML elements using the class="" attribute:

```html
	
<h1 class="company-name">Our Awesome Company</h1>
 
<ul class="unstyled-list">
  <li>Our Work</li>
  <li>About Us</li>
  <li>Give Support</li>
</ul>
```

### Multiple classes
- If possible, it's a good idea to keep your class style rules modular:

```css	
.medium-border {
  border-bottom: 5px grey solid;
}
 
.big-padding {
  padding: 100px;
}
```
- Then, you can combine them by applying multiple classes to the same HTML element:

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

- You can still use them individually elsewhere, too, which helps maintain consistency:

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

### CSS Fundamentals Practice

[CSS Fundamentals workspace in Replit](https://replit.com/@raghubetina1/CSS-Fundamentals)

### External style sheets

- Technically you could write CSS right inside an HTML element using the style="" attribute:

```html
<p style="padding: 100px;">Our mission is to...</p>
```

- As we've seen, it's much more re-usable to define classes. And even better than putting those classes in a `<style>` element within the same HTML document is to put them in an external style sheet.
- Create a file ending in .css and then add a `<link>` element to the HTML file to connect it:

```html
<link rel="stylesheet" href="/my_styles.css">
```

- Now you can easily re-use your rules across all the pages in your site.

[External style sheets workspace in Replit](https://replit.com/@raghubetina1/External-style-sheets)

- We'll be using [Bootstrap](https://getbootstrap.com/) to give us a base of pre-built styles.
- Just need to add [these links](https://chapters.firstdraft.com/chapters/788#quick-links-to-assets) to the `<head>`

### Resources
- [Mozilla Developer Network MDN](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [DevDocs](https://devdocs.io/css/)

## Next Up

[](./)
