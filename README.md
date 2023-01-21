# Styling Buttons

The first thing to know about styling a `<button>` is that it's a regular old
HTML element like any other. Any style that you could apply to a `<div>`, `<p>`,
or `<img>` tag, you can apply to a `<button>`.

"But Chris," you say, "how come it has that box around it and is all grey and
stuff?"

First off, please don't interrupt. But to answer your question, every HTML
element comes with its own default CSS rules already applied! You can see this
for yourself if you fire up an HTML page without adding any CSS rules to it,
then looking at the "Styles" section under the "Elements" tab in your dev tools.
Copy and paste the following into a new HTML file then open it up in your
browser:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Styling Buttons</title>
  </head>
  <body>
    <h1>An h1 element!</h1>
    <p>A p element!</p>
    <button>A button!</button>
  </body>
</html>

```

As you can see, the `<h1>`, `<p>`, and `<button>` elements all have some
built-in styles but while the number of styles applied to the first two is
fairly small, there's a giganto list of styles applied to the `<button>`.

Let's link our HTML to a stylesheet like so:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <link rel="stylesheet" type="text/css" href="style.css"/>
    <title>Styling Buttons</title>
  </head>
  <body>
    <h1>An h1 element!</h1>
    <p>A p element!</p>
    <button>A button!</button>
  </body>
</html>
```
Then create `style.css` and give the page a little color:

```css
body {
  background: #6e98dd;
}
```
If we want to style up our button, we can select it by the tag, make up a class,
an id... anythingc we could do with any other element. Let's select all buttons
and change the border a little bit by adding the following to the botom of our
CSS file:

```css
button {
  border-color: red;
  border-radius: 25%;
}
```

Cool! Let's add more!

```css
button {
  border-color: red;
  border-radius: 25%;
  padding: 20px;
  font-size: 20px;
  color: blue;
}
```
You can change it up like anything else. To paraphrase Bob Ross, "the website is
your canvas. You have total power here!"
