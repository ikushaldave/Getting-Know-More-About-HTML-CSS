### Introduction to Web

Before we begin to learn about HTML and CSS let's see some of the basic concepts of web development. Like what is web development, how a website work, what are the things behind the scene, etc.

To understand this let's take an example.

Let's open a website, say facebook.com, one of the most popular websites. As we hit the URL facebook.com on our browser, we get the Facebook login page. The page looks something like this:

![alt text](https://raw.githubusercontent.com/suraj122/AC-STYLE-images/master/introduction/fb-login.png)

Here we have login form, signup form, facebook image, etc. But, the question is from where we got this page? From where we are getting all these data, like login form, signup form, etc. Let's understand the process.

Actually, the whole website process consists of two parts.

1. CLIENT
2. SERVER

The **CLIENT** can be our computer, or mobile or a web browser on which we can interact with the websites, and from where we are getting all these data is the **SERVER**.

---

![alt text](https://raw.githubusercontent.com/suraj122/AC-STYLE-images/master/introduction/client-server.png)

---

So, whenever we open a website, we make a request to the **SERVER** from the **CLIENT** and the server in response send us the requested page or data.

Here in our case, as we hit the URL facebook.com, we made a request to the server on our browser(Client). And the server in response sends us the Facebook login page. Now If we will put our credentials and click login, we will make another request to the server. And the server will again respond with the Facebook post page if the credentials are correct or else it will throw an error message.

This is how actually, websites works. Every time we make a request to the server and server responds with the requested page.

The basic interactions of **CLIENT** and the **SERVER** are the core element of web development. Based on that, the field of web development is divided into two parts. **Front-end** and **Backend**. CLIENT is the front-end part and SERVER is the backend part.

#### CLIENT(FRONTEND)

The client or the front-end is the user-facing side, where users interact with the websites or applications.

Your computer, mobile devices, web browsers(Safari, chrome, firefox, IE) etc are known as the client.

The languages or the technologies used for client-side programming are:

1. HTML
2. CSS
3. JavaScript.

Generally, those who work on the client-side programming are known as **Front-end Developer**. So, Whatever you see and use, such as the visual aspect of the website, the content like text or images, the interactivity on a page, are all brought together by a front developer.

#### SERVER(BACKEND)

In a simplest word, Backend or the Server is basically a computer located somewhere in the world most likely you can say a **datacenter**. This is where all the data are stored. Sometime the Backend or the Server also known as **Cloud**.

> The backend of the web consists of a server that hosts the website, an application to run it and a database to store the data.

The languages or the technologies used for backend or server-side programming are PHP, Java, JavaScript(node.js), Ruby, Python, etc.

By now you might have guessed, those who work on the backend part are generally known as a **Backend Developer**. Backend developers work behind the scenes, which you don't see on a page or a website.

Role of a Backend Developer

- Develop server-side logic.
- Manage database connections.
- Design APIs.
- Handle security and authentications.
- etc.

You may find some of the above terms fancy, but don't worry you will get familiar to everything slowly slowly.

That's all about the basics of web development, where we have seen about the CLIENT and SERVER. How they are connected and the languages concerned with both CLIENT as well as SERVER.

### Introduction to Web Programming Language

Having the idea, how a website work is great, but it will be more fun when you will know how a website is built and create one of your own. To build a website we have different programming language. We have already seen above that we have some Frontend language and some Backend languages. Anyway here I am not going to discuss anything about the Backend part, so let's not worry about the backend part. Mainly for now we will be focusing on the front-end part of web development.

From the previous discussion, you must be having the idea that there are only three Client-side programming languages(HTML, CSS, and, JavaScript). Let me remind you once again, every time I say, client, it means either a laptop or desktop or mobile or a platform where you can open and interact with websites. In any of these platforms, you can go to your browser and open a website.

Most of the websites are run by only three languages(HTML, CSS & JavaScript) and your browser also understands only these languages only. It is important to note that the browsers understand only **HTML, CSS and JavaScript**. So whatever you see on a page or you interact with it is HTML, CSS, and JS only. It can be said that these three are building blocks of any website. Mostly all the websites rely on these three languages.

As we know that, HTML, CSS, JS, are the only languages used for **front-end** development, now its time to take a deep dig into these languages. Let's see their role one by one and also understand how they are related to each other and what's the difference between them.

### Difference between HTML, CSS & JavaScript.

These languages are closely related to each other but entirely different from each other. Each of them is designed for a specific task. And our goal is to understand their interaction with each other and how they work individually.

Now let's see them individually. But yeah before going one by one let's make an important note i.e. HTML & CSS are not considered as a programming language. HTML is considered as a markup language, which is solely responsible for the content on a page. CSS is just the styling information of the content. But yeah JavaScript is considered a true programming language.

HTML(Hyper Text Markup Language) marks up the raw content with an exact meaning and provide a simple structure to a website.

CSS(Cascading Style Sheet) styles or format those marked-up content.

JavaScript provides interaction with those styled and marked up content.

---

![alt text](https://raw.githubusercontent.com/suraj122/AC-STYLE-images/master/introduction/html-css-js.png)

---

So far so good, we have just learned the difference between HTML, CSS, and, JS. Now, it's time to build something, it's time to code. We will start with HTML & CSS. Once you learn to work HTML & CSS and can build a page using HTML & CSS, then we will learn to make a page interactive using JavaScript. So, let's get started with **HTML & CSS**.

### Introduction to HTML

As of now, we know the role of HTML. We also know it is a markup language. But why it is considered as a markup language, not a programming language? Actually, whatever kind of content we see on a page, it can be anything maybe a paragraph or an image, or a video or a button or anything, to show all these types of content in a browser, HTML is responsible. To see any kind of content on a page we will have to send through HTML only. We need to wrap the content inside HTML, only then the browser will understand what kind of content you are sending. This wrapping the content inside HTML is known as markup. Let's take an example to make it more clear.

Just consider a newspaper article. If you have been asked just mark up each and every section in the article. Obviously, you will start from the top, for heading, you will say it as a heading, then some paragraphs, if there will be any image you will mark it as an image, then again maybe a few more paragraphs, or maybe some quotes inside the article. I will also do the same thing. That's exactly what HTML does. HTML mark up every type of content with the help of elements, tags, and attributes available inside it. So, whatever kind of content we want on a page, we will mark it up with the help of available elements and tags in HTML.

### Elements, Tags, and Attributes.

Now we know how content comes on a page. We also know what is the meaning of markup. To markup different kinds of content in HTML there are different elements. For e.g.: for a paragraph, we have a 'p' element, for an image we have 'img' element, for an article we have 'article' element. Similarly, there are lots of elements based on kind of content, we have div, section, header, nav, button, etc.

#### Elements

Elements are the basic building blocks of HTML. Let's see one of the most common elements used in HTML.

```
<p>Introduction to HTML & CSS</P>
```

The above code is for a paragraph element, wrapping the content _Introduction to HTML & CSS_. Let's break it down.

Here 'p', is the element name.

#### Tags

Once we wrap the element name in between the less than(<) and greater than(>), angle bracket then it becomes a tag. Tags mostly appear within a pair of opening and closing tags.

Opening Tag, from where an element begins. It contains element name in between less than and greater than angle bracket. For example, `<p>`

Closing Tag, this is where an element ends. It is similar to opening tag only, except it contains a forward slash before the element name. For example, `</p>`

In between the opening and closing tags our content comes. For example, _Introduction to HTML & CSS_ is our content.

---

![alt text](https://raw.githubusercontent.com/suraj122/AC-STYLE-images/master/introduction/elem-tag.png)

---

#### Attributes

An element may consist of attributes also. Attributes provide some extra information about the element, which actually doesn't appear as content on a page. Let's see an element that always appears with an attribute.

```
<a href="https://altcampus.io/">AltCampus</a>
```

An attribute always comes within the opening tag after the elements name. It has a name and value. Here in this case 'href' is the name and 'https://altcampus.io/' is the value.

---

![alt text](https://raw.githubusercontent.com/suraj122/AC-STYLE-images/master/introduction/attribute.png)

---

Few more common attributes are 'id' attribute, which identifies an element, 'class' attribute which classifies element, 'src' attribute which specifies the source of embedded content.

Example of Elements: div, section, img, span, strong and many more. The list is really long. No worries as we move further will cover everything.

### Setting up The Standard HTML Document Structure(DOCTYPE, HTML, head, body)

Let's put the things together and create our first web page. For that, we need to set up an HTML document.

HTML documents are simply a plain text editor saved with a `.html` file extension. Let's create a folder and open it in a text editor, it can be any. Either **Sublime** or **VS Code** or **Atom** or whatever you prefer. Create a file inside the folder and save it with .html extension. Let's start the coding part now

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>Hello World</title>
  </head>
  <body>
  </body>
</html>
```

The above line of codes is the standard HTML document structure, which you'll require every time, whenever you'll create a new page or a new document. This is the required structure.

#### !DOCTYPE html

This is the document type declaration, which informs the browser which version of HTML being used and it is always placed at the beginning of the HTML document. There are a number of HTML version, for example, HTML, HTML 4.01, XHTML, HTML5, etc. HTML5 is the latest version and it is declared by `<!DOCTYPE html>`. For a different version, there is a different declaration.

#### html

It signifies the starting of the document. From here the real html document starts. It is also known as the root element of the document. So whatever things we will need to create a page, everything will be coming inside the html i.e, `<html></html>`. Inside html tag `<head></head>` and `<body></body>` element comes.

#### head

Head stores the extra information for a page. For example, the title of the page, metadata(another extra information on the page).

Here we have 'Hello World' as the title of the page.

`<meta charset="utf-8">`, this tells the character encoding of the page.

There are many more tags which comes inside the `<head>` element, we will see as we move further. One of the important points to note here is, whatever comes inside `<head>` element won't be visible on the page.

#### body

All the visible content will come inside the `body` element. So whatever you would like to see on a page, keep them inside the `<body></body>` tags.

Let's open the HTML document in a browser. Once you open the document, you won't see anything on the browser. Because there is nothing inside the `<body></body>` tags. Let's write something inside it.

```
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="utf-8">
      <title>Hello World</title>
    </head>
    <body>
      <h1>Hello World!</h1>
      <p>Our first web page.</p>
    </body>
  </html>
```

Save the document again and refresh your page. Now you'll get to see something. That's exactly how we put content on a page. Here we have, `<h1>Hello World!</h1>`, working as a heading element and `<p>Our first web page.</p>` as a paragraph element.

#### Self Closing Elements

If you recall, earlier we have discussed that elements always appear within a pair i.e. with an opening and closing tags. But, in the previous code snippets have a look of 'meta' tag, you won't find any closing tag. This type of tag is known as a self-closing tag. There are some elements that don't require to be closed. They simply get their content from the attribute within a single tag.

Some of the example of self closing tags are:

`<br>, <hr>, <img>, <input>, <link>, <meta>` etc.

#### Nesting and Indentation

When an element is placed inside another element known as nesting. Here if you look closely in the above line of codes, you'll see that the `<head>` and `<body>` elements are in between the opening and closing tag of html elements. This means that the head and body elements are nested inside the html elements. When any elements are nested inside other elements we also say parent and children relationships. In our case head and body are the children of the html element. And to keep the code more organized and legible and also to differentiate between the child and parent we use indentation. Indentation is just placing some amount of space to the children from its parents. It can be 2 spaces or 1 tab depending upon programmer to programmer.

