# HTML Class 2 — Lists and Images

## What We Learned

In this class, we continued learning HTML. We learned how to create ordered lists, unordered lists, and add images to a web page.

## 1. Ordered List

An **ordered list** displays items in a sequence, usually with numbers. We create it using the `<ol>` tag. Each item goes inside an `<li>` tag.

Example:

```html
<h2>My Daily Routine</h2>
<ol>
    <li>Wake up</li>
    <li>Have breakfast</li>
    <li>Attend class</li>
    <li>Practice coding</li>
</ol>
```

Use an ordered list when the order of the items matters, such as steps in a recipe or instructions.

## 2. Unordered List

An **unordered list** displays items with bullets instead of numbers. We create it using the `<ul>` tag. Each item goes inside an `<li>` tag.

Example:

```html
<h2>My Favourite Fruits</h2>
<ul>
    <li>Apple</li>
    <li>Mango</li>
    <li>Banana</li>
    <li>Orange</li>
</ul>
```

Use an unordered list when the order of the items does not matter, such as a list of hobbies, fruits, or skills.

### Quick Difference

- `<ol>` = ordered list (numbered items)
- `<ul>` = unordered list (bulleted items)
- `<li>` = list item (one item inside either list)

## 3. Adding an Image to an HTML Page

We can add an image to a web page using the `<img>` tag. The `<img>` tag does not need a closing tag.

Two important attributes are:

- `src` — tells the browser where the image is located.
- `alt` — gives a text description of the image. It is useful if the image cannot load and for people using screen readers.

Example:

```html
<img src="flower.jpg" alt="A beautiful flower">
```

This example assumes that `flower.jpg` is saved in the same folder as your `index.html` file.

## 4. Method One: Add an Image Saved on Your Computer

You can save an image to your computer and use it in your HTML page.

### Steps

1. Create a project folder, for example `my-first-website`.
2. Save your HTML file inside this folder as `index.html`.
3. Create an `images` folder inside `my-first-website`.
4. Save your image inside the `images` folder. For example, `flower.jpg`.
5. Add this code to your HTML file:

```html
<img src="images/flower.jpg" alt="A beautiful flower">
```

Your folder structure should look like this:

```text
my-first-website/
├── index.html
└── images/
    └── flower.jpg
```

**Important:** The file and folder names in `src` must match the actual names. Check the file extension too, such as `.jpg`, `.png`, or `.webp`.

## 5. Method Two: Add an Image Using an Online URL

You can display an image from a website by using its direct image URL.

### Steps

1. Find an image on a website or through Google Images.
2. Open the image or use the website's option to copy the image address.
3. Copy the **direct URL of the image**, not just the Google search results page or the website's normal page URL.
4. Put the URL inside the `src` attribute.

Example:

```html
<img src="https://example.com/images/flower.jpg" alt="A beautiful flower">
```

The URL above is only an example. Replace it with the actual direct image URL you want to use.

### If the Online Image Does Not Appear

- Check that the URL is correct.
- Check that you copied the image URL, not the search page URL.
- Some websites do not allow their images to be displayed on other websites.
- The image may have been moved or deleted.
- For your own projects, saving the image in your project folder is often more reliable.

**Reminder:** Use images you have permission to use. Do not assume every image found through Google is free to reuse.

## 6. Complete Example

Try this example in your `index.html` file. Replace the image path with your own image file or a direct online image URL.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Favourite Things</title>
</head>
<body>
    <h1>My Favourite Things</h1>

    <h2>My Hobbies</h2>
    <ul>
        <li>Reading</li>
        <li>Playing cricket</li>
        <li>Learning coding</li>
    </ul>

    <h2>My Daily Routine</h2>
    <ol>
        <li>Attend class</li>
        <li>Practice HTML</li>
        <li>Complete homework</li>
    </ol>

    <h2>My Favourite Image</h2>
    <img src="images/flower.jpg" alt="A beautiful flower">
</body>
</html>
```

## Class Practice

Create a web page that includes:

1. A main heading.
2. An unordered list with at least four favourite things.
3. An ordered list with at least three steps for a daily task.
4. One image saved in your project folder **or** one direct online image URL.
5. An appropriate `alt` description for the image.

Save the file as `index.html` and open it in your browser to check your work.

## Key Takeaways

- Use `<ol>` for numbered lists.
- Use `<ul>` for bulleted lists.
- Use `<li>` for each list item.
- Use `<img>` to display an image.
- Use `src` to specify the image location.
- Use `alt` to describe the image.
- A local image path must match your folder structure and file name.
- An online image needs a direct image URL that is accessible.

Keep practising by changing the list items and trying different images.
