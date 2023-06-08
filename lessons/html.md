# HTML
This lesson goes over HTML: why and how we use it

<!-- TODO -->
## [Slides](../slides/html/index)

## Topics
- HTML

## Story
- Emily wanted to share her stories with the world 🌍📚
- She discovered the power of the internet and decided to create a website for publishing her stories 🌐📖
- Emily realized that plain text wasn't engaging enough and turned to **HTML**, the magical language for creating webpages ✨💻
- HTML allowed Emily to add structure and meaning to her content using tags like **headings** `<h1>`, **paragraphs** `<p>`, bold `<b>`, and italic `<i>` 🏷️📝
- Emily discovered the magic of hyperlinks, using the `<a>` tag, which connected her readers to new adventures and ideas 🌐🔗
- With each hyperlink, Emily's stories came alive on the web, creating an enchanting world of imagination 📚✨
- HTML transformed Emily's stories from hidden notebooks to captivating and interactive experiences on her website 📖🌈

## HTML (HyperText Markup Language)
- **HyperText** is a fancy word for text with links
- **Markup** means we can add symbols to control formatting and structure


## HTML Syntax

```html
<a href="https://www.wikipedia.org">
  Go to Wikipedia
</a>
```

- Opening tag `<a>`
- Closing tag, `</a>`
- Content in between, `Go to Wikipedia`
- Attributes inside the opening tag, `href=""`
- Collectively, we call this an **element**


### Elements can have more than one **attribute**.

```html
<a href="https://www.wikipedia.org" target="_blank">
  Go to Wikipedia
</a>
```


### Elements can contain other elements.

```html
<!-- parent -->
<a href="https://www.wikipedia.org" target="_blank">
  <!-- child -->
  <img src="/wikipedia.jpg" alt="Go to Wikipedia">
</a>
```

1. In that case, the one inside is known as a **child element** and the one outside is the **parent element**.

2. If there are multiple levels of **nesting**, then all the elements inside an outer element are its **descendants**.


## Attributes

Most attributes only make sense on specific elements.

1. `href=""` is for `<a>` elements, to specify where to take the user when they click the link.
2. `src=""` is for `<img>` elements, to specify the url of the image to load.
3. `for=""` is for `<label>` elements, to specify which input element it is paired with.

- Some attributes can be put on almost any element, like `class=""` or `id=""`
- An **id** should only be used once per document.
- A **class** can and should be used repeatedly.

## HTML Boilerplate

- **boilerplate** - code that can be used over and over again
- A html document has 1 *body* and 1 *head* tag. (only 1 of each)
- Think of it like a person. I can't see what's going on inside your *head*, but I can see your *body*.
- We put things like links, titles, and rules in the *head*. What gets rendered in the browser goes in the body.

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

## Replit

- You'll need to sign up for a [Replit](https://replit.com/) account, a cloud-based code editing environment
- You can sign in with your GitHub account if you want.
- Click the blue "Fork REPL" button in the top-right corner to get a workspace to play around in.
- Read the code, modify the code, play around and make sure that you understand every single line. Ask any questions that occur to you.

- [Basic HTML Content Replit Workspace](https://replit.com/@raghubetina1/Basic-content)
- [HTML Lists Replit Workspace](https://replit.com/@raghubetina1/Lists)


## Forms
- There's one more essential element `<form>`.
- We can't really do anything with forms right now, since HTML can't process input — it's a formatting language.
- We'll learn about forms after we learn enough Ruby and Ruby on Rails to do things with user input.

## Resources

[Mozilla Developer Network, MDN](https://developer.mozilla.org/en-US/)

[DevDocs](https://devdocs.io/html/)

## Next Up

[CSS](./css)
