# Background Images

This repository contains the starter files for the Background Images coding exercise in Web Design 1.

In this exercise, you will learn how to add images with CSS instead of adding them directly in the HTML. So far, you have used background colors to style different parts of a page. Background images work in a similar way, but they give you more visual options for adding texture, decoration, patterns, headers, and subtle design details.

The goal of this exercise is to understand the basic CSS properties used for background images and how those properties affect the way images appear inside different HTML elements.

---

## Use Canvas for the Full Assignment Instructions

Canvas has the full assignment description, screencast video, due date, and submission instructions.

This README is here to explain the project, remind you of the major concepts, and help you check your work before submitting.

Follow the Canvas instructions and watch the screencast video carefully.

---

## Important GitHub Workflow

This assignment uses GitHub.

You will need to:

1. Create or open your own repository for this exercise.
2. Clone the repository to your computer using GitHub Desktop.
3. Open the full project folder in Visual Studio Code.
4. Complete the Background Images exercise.
5. Save your files.
6. Commit your changes in GitHub Desktop.
7. Push your changes to GitHub.
8. Publish the site using GitHub Pages.
9. Add the published GitHub Pages link to the About section of your repository.
10. Submit the URL of your GitHub repository in Canvas.

The submitted Canvas link should be the **repository** URL, not the published GitHub Pages website URL.

---

## What You Will Practice

By completing this exercise, you will practice how to:

- Add background images with CSS
- Use the `background-image` property
- Use the `url()` function to connect to an image file
- Understand how background images are different from HTML image elements
- Add a repeating background texture to the `body`
- Add a larger background image to a `header`
- Control whether a background image repeats
- Use `background-repeat`
- Use `background-size`
- Compare `cover` and `contain`
- Set a background image to a specific pixel size
- Use `background-position`
- Move a background image to places like the bottom right corner
- Use padding to move text away from a background image
- Understand why margin and padding affect background images differently
- Add decorative watermark-style images to page sections
- Commit and push changes to GitHub
- Publish the finished page with GitHub Pages

---

## Background Images vs. HTML Images

You have already used the HTML `img` element to add images to a page.

HTML images are part of the page content. They take up space in the document and can include important information for the user.

Background images are different. They are added with CSS and are usually decorative. They appear behind the content inside an element.

For example:

- Use an HTML `img` element when the image is part of the meaning or content of the page.
- Use a CSS background image when the image is mostly decoration, texture, pattern, or visual styling.

In this exercise, the background images are being used for decoration and design.

---

## Adding a Background Image

The basic property for adding a background image is:

- `background-image`

The value uses the `url()` function.

Example:

    background-image: url(tile.png);

The image filename goes inside the parentheses.

If the image is in the same folder as the CSS file, you can usually use just the filename. If the image is inside another folder, such as an `images` folder, you need to include the folder name in the path.

Example:

    background-image: url(images/tile.png);

The path must match the actual folder and filename exactly.

---

## Repeating Background Images

By default, background images repeat.

That means if the image is smaller than the area it fills, the browser will repeat the image horizontally and vertically.

This works well for small texture images or seamless patterns. A seamless pattern is designed so the edges match up when the image repeats.

In this exercise, you will add a repeating background image to the `body` element. Since the `body` represents the page area, the background texture can fill the entire browser window.

---

## Background Images on the Body

The `body` element represents the main visible area of the page.

When you add a background image to the `body`, the image can appear across the whole browser window.

A small repeating texture can work well here because it can fill a large area without needing a huge image file.

The idea is to create visual texture without distracting from the content.

---

## Background Images on the Header

You will also add a background image to the `header`.

This is a little different from the body background because the header is a smaller area of the page.

If the image is larger than the header, the browser may only show part of the image. That can be fine when the image is being used as a decorative background.

A background image does not push text out of the way. The text and image can occupy the same space. That is useful, but it also means you need to make sure the text remains readable.

---

## Background Images on Headings

You will add a small image to heading elements such as `h2`.

This introduces an important challenge: the image may appear behind the text.

If the background image overlaps the words, the heading may become hard to read.

One way to fix that is with padding.

For example, if the image appears on the left side of a heading, you can use left padding to move the text over:

    padding-left: 40px;

This works because padding adds space inside the element. The background image remains part of the element, but the text moves inward.

Margin would not solve this problem in the same way because margin moves the entire element, including the background image.

---

## Margin vs. Padding with Background Images

This exercise is a good reminder of the box model.

Margin is outside the element.

Padding is inside the element.

Background images are part of the element’s box. That means:

- If you add margin, the whole element moves.
- If you add padding, the content inside the element moves.

When you need to move text away from a background image, padding is usually the better choice.

---

## Controlling Image Size

You will use the `background-size` property to control how large a background image appears.

Common values include:

- `cover`
- `contain`
- pixel values, such as `75px`
- percentage values

### `cover`

The value `cover` makes the image large enough to cover the entire element.

This can be useful for large decorative areas, but part of the image may be cropped.

### `contain`

The value `contain` makes the whole image visible inside the element.

This can be useful when you need to see the entire image, but it may leave extra space or cause repeating if repeat is still turned on.

### Pixel Sizes

You can also set the background image to a specific size.

Example:

    background-size: 75px;

This can be useful for small icons, watermark images, or decorative graphics.

---

## Controlling Repeating

You will use the `background-repeat` property to control whether a background image repeats.

Useful values include:

- `repeat`
- `no-repeat`
- `repeat-x`
- `repeat-y`

### `repeat`

This is the default. The image repeats horizontally and vertically.

### `no-repeat`

The image appears only once.

### `repeat-x`

The image repeats horizontally.

### `repeat-y`

The image repeats vertically.

If a background image is repeating when you do not want it to, add:

    background-repeat: no-repeat;

---

## Controlling Position

You will use the `background-position` property to move a background image inside an element.

You can use keywords such as:

- `top`
- `bottom`
- `left`
- `right`
- `center`

You can also combine keywords.

Example:

    background-position: bottom right;

This places the background image in the bottom right corner of the element.

This is especially useful for decorative watermark-style images.

---

## Watermark-Style Background Images

In this exercise, you will add a subtle background image to repeated page sections.

This kind of background image is often used as a watermark. It is not the main content of the page. It is just there to add a little visual interest.

For a watermark-style image, you will usually want to control:

- size
- repeat
- position

A typical pattern might include:

    background-image: url(watermark.png);
    background-size: 75px;
    background-repeat: no-repeat;
    background-position: bottom right;

This keeps the image subtle and places it in a consistent location.

---

## Background Image Shorthand

CSS also has a shorthand `background` property that can combine several background settings into one line.

However, in this exercise, we are keeping the properties separate so the purpose of each property is easier to understand.

You will mostly use properties such as:

- `background-image`
- `background-size`
- `background-repeat`
- `background-position`

Writing them separately is a good choice while you are learning because it makes the code easier to read and troubleshoot.

---

## File Naming Reminder

Background image files should be named clearly.

In the video, background image filenames may use a prefix such as `bkg_`.

That kind of naming pattern can be helpful because it keeps background images grouped together alphabetically in the file list.

Examples:

- `bkg_header.png`
- `bkg_texture.png`
- `bkg_watermark.png`

You do not need to rename the starter files, but pay attention to the exact spelling of each filename.

Filenames matter. `tile.png`, `Tile.png`, and `tile.PNG` may not be treated the same way on every system.

---

## Accessibility Reminder

Background images are usually decorative.

Because they are added with CSS, they do not have `alt` text like an HTML image.

That means you should not use a CSS background image for important content that users need in order to understand the page.

If the image communicates important information, use an HTML `img` element with appropriate `alt` text instead.

For this exercise, the background images are decorative.

---

## Before You Submit

Before submitting your work in Canvas, check the following:

- You opened the full project folder in Visual Studio Code
- Your CSS file is linked correctly
- The background texture appears on the body
- The header has a background image
- The heading background image appears only once
- The heading text is still readable
- Padding is used where needed to move text away from a background image
- The section backgrounds include a subtle watermark-style image
- The watermark image is sized appropriately
- The watermark image does not repeat
- The watermark image is positioned where you want it
- The page looks correct when opened in a browser
- You saved your files
- You committed your changes in GitHub Desktop
- You pushed your changes to GitHub
- You published the site with GitHub Pages
- You added the GitHub Pages link to the About section of your repository
- You are submitting the GitHub repository URL in Canvas

---

## What to Submit

Submit the URL of your GitHub repository in Canvas.

Do not submit a ZIP file.

Do not submit only the GitHub Pages URL.

Your Canvas submission should look something like:

- `https://github.com/your-username/background-images`

The GitHub Pages URL should be added to the About section of the repository, but the repository URL is what should be submitted in Canvas.

---

## Suggested Commit Message

A good commit message for this exercise might be:

- `Completed background images exercise`

You do not need a long commit message. A short, clear summary is enough.

---

## Troubleshooting Tips

If something is not working, check these common issues first.

### My background image is not showing

Check:

- Did you save the CSS file?
- Is the CSS file linked correctly in the HTML?
- Is the image filename spelled correctly?
- Is the image file in the correct folder?
- Does the path inside `url()` match the actual file location?
- Did you include the parentheses in `url()`?
- Did you forget a semicolon?

### My image is repeating too much

Background images repeat by default.

Add this if you only want the image to appear once:

    background-repeat: no-repeat;

### My image is too large or too small

Use `background-size`.

Try values such as:

    background-size: cover;

    background-size: contain;

    background-size: 75px;

### My image is in the wrong place

Use `background-position`.

Example:

    background-position: bottom right;

You can also try values such as:

- `center`
- `top right`
- `bottom left`

### My text is hard to read

Background images can appear behind text.

Try:

- using a subtler image
- changing the text color
- adding padding
- adding a background color
- choosing a different background position

Remember that readability is more important than decoration.

### My repository does not show my latest work

Check GitHub Desktop.

You may have saved your files locally but forgotten to commit or push.

Remember:

- Save updates files on your computer.
- Commit creates a checkpoint.
- Push uploads that checkpoint to GitHub.com.

If you forget to push, your instructor may only see the older version of your project.

### My GitHub Pages site does not update immediately

GitHub Pages may take a little time to rebuild after you push changes.

Wait a minute or two, then refresh the published site.

Also make sure your repository includes an `index.html` file at the correct location.

---

## Final Reminder

Background images can make a page look more polished, but they should support the design instead of distracting from the content.

Use them thoughtfully.

The most important pattern to remember is:

1. Choose the element that should receive the background image.
2. Add `background-image` with `url()`.
3. Control the size with `background-size`.
4. Control repeating with `background-repeat`.
5. Control placement with `background-position`.
6. Check that the page is still readable.
