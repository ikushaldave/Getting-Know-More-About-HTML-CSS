### Introduction to CSS

Great, now you have the basic knowledge of HTML. In the previous section, you learned to put the content on a page. Remember HTML defines only the content of a page and gives you a very simple structure. Now its time to switch our gear to CSS and style our page. CSS will define the visual styles and appearance of our page.

To style our element on a page, we need to first target the element and then define our styles. And for this purpose, we have, `selectors, properties and values` in CSS.

### 9. Selectors, Properties, and Values.

Suppose we want to change the color and font size of the heading on our page that we have created just a few minutes ago. So we need to target the `h1` element. Let's see how we do this.

```
h1 {
  color: red;
  font-size: 34px;
}
```

#### Selectors:

Here 'h1' is working as a selector. This is how we target an element within CSS. There are other ways also to target an element. But first, let's understand the above code then we will move further. So, once an element is selected then its style can be defined inside the curly braces `{.......}`.

#### Properties & Values:

Here 'color' & 'font-size' are the properties of the element we targeted and 'red' & '34px' are the values. Property determines the style that needs to be applied and value determines the behavior of the property. It can be any property & value of the element. for example, `background-color: blue, width: 300px, height: 300px, position: fixed`, etc. It depends on what we want to style.

---

![alt text](https://raw.githubusercontent.com/suraj122/AC-STYLE-images/master/introduction/styles.png)

---

### Types of Selectors(Type, Class, ID)

Above we learned to target our element and style it. That's one way. Let's see all other ways that can be used to target the element in CSS.

#### Type Selector:

Type selectors target an element with the element name or element type. For example,

```
h1 {
  color: red;
  font-size: 34px;
}
p {
  background-color: green;
  color: red;
}
div {
  width: 400px;
  height: 300px;
}
```

Here `h1 , p, div` are the name or types of elements that we use in HTML. We can have different types of elements based on the types of contents we need. The thing is that if we target using the element's name or element type, each element of that type will be targeted at once. For example, say we have four `ps` in our html document. Now if we target the `p` element using its name, so all the four `ps` will be styled. That's why we call it type selector.

But, suppose if we want to target just one `p` at a time, not all, so for that purpose, we have `class and id` selector.

#### Class Selector:

Class Selector allows us to target an element with the class attribute defines inside the tag. For example,

```
<div class="box">........</div>

.box {
  height: 150px;
  width: 150px;
  background-color: red;
}
```

To represent a class selector in CSS we denote it with `.` followed with the value we define inside the class attribute. Here, `box` is our class selector and it will select the element containing the class attribute value of `box`. We are free to choose any class name. And also at one time, we can provide the same class name to different elements.

For example:

```
  <div class="perfect">.........</div>

  <p class="perfect">.........</p>

  .perfect {
    text-align: center;
  }
```

Here, the `perfect` class selector will select both `div and p` elements. The class selector is more specific than the type selector. Because with class selector we can target some particular number of elements instead of all the elements of one type.

#### ID Selectors:

An ID selector is even more specific than class and type selector. Because we can target only one unique element at a time. As we define a class attribute similarly we define ID attribute inside a tag. But to target an element using an ID selector in CSS we use `#` followed by the value defined inside the ID attribute.

For example:

```
  <div id="altcampus"></div>

  #altcampus {
    background-color: green;
  }
```

Here, `altcampus` is the ID selector and it will only select the element containing the id attribute value of `altcampus`.

One important point to be noted here is that an ID attribute value can be used once per page. It has to be unique. We can't reuse the same ID attribute value for other elements on the same page.

### Referencing CSS

It's time to connect the dots. We have the basic idea of HTML & CSS. We know how to define content in html and also how to style the element. So, let's connect them.

You can take three different approaches to connect the HTML and CSS. `Internal and Inline` styling that can be written HTML document only. The best practice is to create an `external stylesheet` and then connect them.

#### Inline Styling

In inline styling, we write our style inside the tag only. For example:

```
  <div style="background-color: red; color:blue; ">.......</div>
```

#### Internal Styling

For internal styling, we define a style tag inside the head element of the document and then we write our CSS.

For example:

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>Hello World</title>
    <style>
      body {
        background-color: green;
      }
      .heading {
        color: black;
        font-size: 36px;
      }
    </style>
  </head>
  <body>
    <h1 class="heading">Hello World!</h1>
    <p>Our first web page.</p>
  </body>
</html>
```

#### External Stylesheet

The best practice is to have one separate stylesheet to write our CSS and then connect it with the `link` tag inside the head elements.

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>.......</title>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <h1 class="heading">Hello World!</h1>
    <p>Our first web page.</p>
  </body>
</html>
```

To create an external stylesheet, let's just open the same folder we have created earlier in our text editor. Now create a new file with extension `.css` in the same folder. After that connect the CSS file to HTML document in a similar way we have done in the about code snippet. And in the CSS file, we can normally target any element and style according to the need.

```
body {
  background-color: green;
}
.heading {
  color: black;
  font-size: 36px;
}
```

External stylesheet helps us in organizing both HTML & CSS code separately. And it also helps us in styling the entire website using just a single stylesheet. For separate pages, we won't have to write CSS separately. With just a single stylesheet we can style all the pages on a website.
