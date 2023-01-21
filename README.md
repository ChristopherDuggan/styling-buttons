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

As you can see, the `<h1>`...
![Screenshot 2023-01-21 at 15 53 49](https://user-images.githubusercontent.com/27020691/213887578-b33ebfd4-b347-4cef-a30e-38bbea495ae0.png)

`<p>`...
![Screenshot 2023-01-21 at 15 57 17](https://user-images.githubusercontent.com/27020691/213887604-0d3a8996-85ec-4a89-99c4-fbb86709808e.png)![Screenshot 2023-01-21 at 16 09 00](https://user-images.githubusercontent.com/27020691/213887683-ba9d5fe4-4f53-47ec-a94d-f084e222623c.png)


and `<button>` elements...
![Screenshot 2023-01-21 at 15 57 44](https://user-images.githubusercontent.com/27020691/213887586-69618c77-6bb7-49e4-92e5-2b8877a3b1dd.png)


all have some built-in styles but while the number of styles applied to the first two is
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
![Screenshot 2023-01-21 at 16 09 00](https://user-images.githubusercontent.com/27020691/213887689-4cc9f1e7-0677-492a-b7ad-76c5f34d04bf.png)

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

![Screenshot 2023-01-21 at 16 13 17](https://user-images.githubusercontent.com/27020691/213887687-61b76f47-3035-46b0-9828-562449691bed.png)

You can change it up like anything else. To paraphrase Bob Ross, "the website is
your canvas. You have total power here!"

![Bob-Ross-Header-728x409](https://user-images.githubusercontent.com/27020691/213887741-2046459b-2b3e-45de-9393-b2ff99619572.jpg)
