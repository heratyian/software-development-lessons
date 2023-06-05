# HTML
This lesson goes over HTML: why and how we use it

<!-- TODO -->
## [Slides](../slides/html/index)

## Topics
- HTML

<!-- TODO: add story: tie it to a concrete concept that you already understand -->
<!-- You have a bunch of text, but want to connect it to other places. Like a book with annotations. -->

## Story

Once upon a time, there was a talented young writer named Emily. She had a passion for storytelling and had written numerous captivating short stories. However, Emily faced a challenge - her stories remained hidden in notebooks tucked away on her bookshelf.

One day, Emily discovered the power of the internet 🛜. She realized that she could share her stories with people from all around the world 🌎. Excited by the idea, she decided to create a website where she could publish her stories for everyone to read 📖.

But there was a problem. Emily quickly realized that simply posting her stories as plain text on a webpage wouldn't be engaging enough. She wanted her readers to have a more immersive experience. So she turned to a magical language called **HTML**.

HTML, short for Hypertext Markup Language, allowed Emily to enhance her stories. It was a language specifically designed for creating webpages. With HTML, Emily could add structure and meaning to her content.

Emily started by using HTML **tags** to mark up her text. She used **headings** `<h1>` to make her story titles stand out, **paragraphs** `<p>` to organize her thoughts, and even bold `<b>` and italic `<i>` tags to emphasize certain words or phrases.

But the real magic happened when Emily discovered hyperlinks. Hyperlinks were like portals that allowed her readers to jump from one webpage to another with just a click. Emily used the `<a>` tag, short for anchor, to create these hyperlinks. She could link to other stories on her website, external websites for additional information, or even create navigation menus to help her readers explore her collection.

As Emily continued to learn and experiment with HTML, her stories came alive on the web. With each hyperlink, she connected her readers to new adventures and ideas. Her website became a gateway to an enchanting world of imagination, where her readers could lose themselves in her stories.

Thanks to HTML, Emily's stories no longer remained hidden on her bookshelf. And so, the tale of Emily and HTML reminds us that with the power of markup and hyperlinks, we can transform simple webpages into captivating and interactive experiences for our readers.

## HTML (HyperText Markup Language)
- **HyperText** is a fancy word for text with links
- **Markup** means we can add fancy symbols to control formatting and structure


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
