# Starting Your Code - Template 1

## Starting html 

```html 
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My Portfolio</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
```

---

## Navbar - html and css
```html
    <header>
      <div class="navbar">
        <div class="logo">Stellin John George</div>
        <ul class="nav-links">
          <li><a href="#">Home</a></li>
          <li><a href="#">Photo</a></li>
          <li><a href="#">About Me</a></li>
          <li><a href="#">Contact</a></li>
        </ul>
        <div class="menu-icon">
          <span></span>
        </div>
      </div>
    </header>
```

```css
body, html {
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
    background-color: #202020;
    color: white;
}
```
- `padding`: Removes the default padding from both the body and html elements.
- `margin`: Removes the default margin from both the body and html elements.
- `font-family`: Sets the default font style to Arial, with a fallback to sans-serif.
- `background-color`: Sets the background color to dark grey (#202020).
- `color`: Sets the default text color to white.

```css
header {
    background-color: #363636;
    padding: 20px;
    color: white;
    position: fixed;
    width: 100%;
    top: 0;
    left: 0;
    z-index: 1000;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    box-sizing: border-box;
}
```
- `background-color`: Sets the background color of the header to a darker grey (`#363636`).
- `padding`: Adds padding around the header (20px).
- `color`: Sets the text color inside the header to white.
- `position`: Fixes the header at the top of the page.
- `width`: Makes the header span the full width of the page (100%).
- `top`: Positions the header at the top of the page.
- `left`: Aligns the header to the left.
- `z-index`: Ensures the header stays on top of other content (1000).
- `box-shadow`: Adds a shadow below the header for depth (`0 2px 5px rgba(0, 0, 0, 0.1)`).
- `box-sizing`: Includes padding in the element's total width and height (`border-box`).

```css
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 0;
}
```
- `display`: Uses Flexbox to align navbar items (`flex`).
- `justify-content`: Distributes space between the logo and navigation links (`space-between`).
- `align-items`: Vertically centers the items within the navbar (`center`).
- `margin`: Removes any default margin around the navbar (`0`).

```css
.nav-links {
    list-style-type: none;
    display: flex;
    gap: 20px;
    margin: 0;
    padding: 0;
}
```
- `list-style-type`: Removes bullet points from the list (`none`).
- `display`: Uses Flexbox to arrange list items in a row (`flex`).
- `gap`: Adds space between the navigation links (`20px`).
- `margin`: Removes any default margin around the list (`0`).
- `padding`: Removes any default padding around the list (`0`).


```css
.nav-links li {
    display: inline;
}
```

- `display`: Displays list items inline (`inline`).



```css
.nav-links a {
    color: white;
    text-decoration: none;
    font-weight: bold;
    transition: color 0.3s ease;
}
```

- `color`: Sets the text color of navigation links to white.
- `text-decoration`: Removes the underline from links (`none`).
- `font-weight`: Makes the text bold (`bold`).
- `transition`: Adds a smooth transition effect for the color change on hover, taking 0.3 seconds (`color 0.3s ease`).


```css
.nav-links a:hover {
    color: #f0a500;
}
```

- `color`: Changes the link color to a yellowish tone (`#f0a500`) when hovered over.

```css
.menu-icon {
    display: none;
}
```

- `display`: Hides the menu icon (`none`). This can be used to control the visibility of the menu icon, often for mobile view adjustments.

---

## First Div

```html 
    <section class="hero">
      <div class="hero-image">
        <img src="" alt="Portfolio Image" />
      </div>
      <div class="hero-content">
        <h1>
          My <br />
          Portfolio
        </h1>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad
          minim veniam, quis nostrud.
        </p>
        <div class="hero-buttons">
          <a href="#" class="btn">Explore Now</a>
          <a href="#" class="btn-video"><span>&#9654;</span> Play Video</a>
        </div>
      </div>
    </section>
```

```css
.hero {
    display: flex;
    align-items: center;
    justify-content: center;
    height: calc(100vh - 100px);
    background-color: #202020;
    color: white;
    padding: 0 80px;
}
```

- `display`: Uses Flexbox to align elements within the hero section (`flex`).
- `align-items`: Vertically centers the content within the hero section (`center`).
- `justify-content`: Horizontally centers the content within the hero section (`center`).
- `height`: Sets the hero section height to the full viewport height minus 100 pixels (typically to account for the height of a navbar) (`calc(100vh - 100px)`).
- `background-color`: Sets the background color of the hero section to dark grey (`#202020`).
- `color`: Sets the text color within the hero section to white.
- `padding`: Adds horizontal padding of 80 pixels on both left and right sides of the hero section (`0 80px`).


```css
.hero-image {
    flex: 1;
    max-width: 50%;
}
```

- `flex`: Allows the image section to grow and fill available space within the flex container (`1`).
- `max-width`: Limits the width of the hero image section to 50% of its container (`50%`).

```css
.hero-image img {
    width: 100%;
    height: auto;
    border-radius: 10px;
    object-fit: cover;
    padding-top: 100px;
}
```

- `width`: Sets the image width to 100% of its container, ensuring it fills the available space.
- `height`: Adjusts the height automatically to maintain the image's original aspect ratio (`auto`).
- `border-radius`: Rounds the corners of the image by 10 pixels, giving it a softer appearance.
- `object-fit`: Scales the image to cover its container while maintaining its aspect ratio (`cover`).
- `padding-top`: Adds 100 pixels of padding above the image, creating space at the top.


```css
.hero-content {
    flex: 1;
    max-width: 50%;
    text-align: left;
    padding-left: 40px;
}
```

- `flex`: Allows the text section to grow and fill available space within the flex container (`1`).
- `max-width`: Limits the width of the hero text section to 50% of its container (`50%`).
- `text-align`: Aligns the text to the left (`left`).
- `padding-left`: Adds 40 pixels of space between the hero image and the text, providing separation (`40px`).


```css
.hero h1 {
    font-size: 60px;
    line-height: 1.2;
    margin: 0;
}
```

- `font-size`: Sets a large font size for the hero heading (`60px`).
- `line-height`: Sets the line height to 1.2 times the font size, ensuring proper spacing between lines of text (`1.2`).
- `margin`: Removes the default margin around the heading (`0`).


```css
.hero p {
    font-size: 16px;
    margin: 20px 0;
    line-height: 1.6;
}
```

- `font-size`: Sets the font size for the hero paragraph text (`16px`).
- `margin`: Adds 20 pixels of vertical space above and below the paragraph (`20px 0`).
- `line-height`: Sets the line height to 1.6 times the font size, improving readability (`1.6`).


```css
.hero-buttons {
    margin-top: 20px;
}
```

- `margin-top`: Adds 20 pixels of space above the hero buttons, creating separation from the content above (`20px`).

```css
.btn, .btn-video {
    display: inline-block;
    padding: 10px 20px;
    margin-right: 10px;
    background-color: white;
    color: black;
    text-decoration: none;
    font-weight: bold;
    border-radius: 5px;
    transition: background-color 0.3s ease, color 0.3s ease;
}
```

- `display`: Displays the buttons inline, but as blocks, allowing them to have padding and margin (`inline-block`).
- `padding`: Adds padding inside the buttons, 10 pixels vertically and 20 pixels horizontally (`10px 20px`).
- `margin-right`: Adds 10 pixels of space to the right of each button, providing separation between buttons (`10px`).
- `background-color`: Sets the button background color to white.
- `color`: Sets the button text color to black.
- `text-decoration`: Removes the underline from text links within the buttons (`none`).
- `font-weight`: Makes the button text bold.
- `border-radius`: Rounds the corners of the button by 5 pixels, giving it a softer appearance (`5px`).
- `transition`: Adds a smooth transition effect for changes in background color and text color on hover, taking 0.3 seconds (`background-color 0.3s ease, color 0.3s ease`).


```css
.btn:hover {
    background-color: black;
    color: white;
}
```

- `background-color`: Changes the button's background color to black when hovered over.
- `color`: Changes the button's text color to white on hover.

```css
.btn-video {
    background-color: transparent;
    color: white;
    border: 1px solid white;
}
```

- `background-color`: Sets the video button's background to transparent, allowing the background behind it to show through.
- `color`: Sets the text color of the video button to white.
- `border`: Adds a white, 1-pixel solid border around the video button.


```css
.btn-video:hover {
    background-color: #f0a500;
    color: black;
}
```

- `background-color`: Changes the background color of the video button to a yellowish tone (`#f0a500`) when hovered over.
- `color`: Changes the text color of the video button to black on hover.


---
## Second Div

```html
<section class="introduction">
      <div class="intro-content">
        <div class="intro-left">
          <h2>Introduction</h2>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
            aliquip ex ea commodo consequat. Duis aute irure dolor in
            reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
            pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
            culpa qui officia deserunt.
          </p>

          <div class="intro-sub-sections">
            <div class="intro-sub-section">
              <h3>About Me</h3>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
                enim ad minim veniam, quis nostrud exercitation ullamco laboris
                nisi ut aliquip ex ea commodo consequat.
              </p>
            </div>

            <div class="intro-sub-section">
              <h3>About Portfolio</h3>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
                enim ad minim veniam, quis nostrud exercitation ullamco laboris
                nisi ut aliquip ex ea commodo consequat.
              </p>
            </div>
          </div>
        </div>
        <div class="intro-image">
          <img src="" alt="Introduction Image" />
        </div>
      </div>
    </section>
```

```css
.introduction {
    padding: 50px 80px;
    background-color: #202020;
    color: white;
}
```

- `padding`: Adds 50 pixels of padding to the top and bottom, and 80 pixels of padding to the left and right, providing space inside the element (`50px 80px`).
- `background-color`: Sets the background color of the introduction section to dark grey (`#202020`).
- `color`: Sets the text color within the introduction section to white.

```css
.intro-content {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    gap: 20px;
}
```

- `display`: Uses Flexbox to align the introduction content (`flex`).
- `justify-content`: Distributes space between the content elements, placing space equally between them (`space-between`).
- `align-items`: Aligns items to the top of the container (`flex-start`).
- `gap`: Adds 20 pixels of space between the text and image, creating separation (`20px`).


```css
.intro-left {
    flex: 2;
    padding-right: 20px;
}
```

- `flex`: Allows the `intro-left` section to take up more space compared to other flex items, specifically twice as much space (`2`).
- `padding-right`: Adds 20 pixels of space to the right of the `intro-left` section, creating separation between the text and image (`20px`).


```css
.intro-left h2 {
    font-size: 50px;
    margin-bottom: 10px;
    position: relative;
}
```

- `font-size`: Sets a large font size for the heading (`50px`).
- `margin-bottom`: Adds 10 pixels of space below the heading, separating it from subsequent content (`10px`).
- `position`: Sets the positioning of the heading to relative, which allows for additional styling, such as adding an underline or other elements relative to the heading (`relative`).

```css
.intro-left h2::after {
    content: '';
    display: block;
    width: 60px;
    height: 3px;
    background-color: white;
    margin-top: 10px;
}
```

- `content`: Creates an empty content block for the underline (`''`).
- `display`: Makes the pseudo-element a block element, allowing it to take up the full width specified (`block`).
- `width`: Sets the width of the underline to 60 pixels (`60px`).
- `height`: Sets the height of the underline to 3 pixels (`3px`).
- `background-color`: Sets the color of the underline to white.
- `margin-top`: Adds 10 pixels of space above the underline, separating it from the heading text (`10px`).


```css
.intro-left p {
    font-size: 16px;
    line-height: 1.6;
    margin-bottom: 20px;
}
```

- `font-size`: Sets the font size for the paragraph text to 16 pixels.
- `line-height`: Sets the line height to 1.6 times the font size, improving readability.
- `margin-bottom`: Adds 20 pixels of space below each paragraph, separating it from the next element.


```css
.intro-sub-sections {
    display: flex;
    justify-content: space-between;
    gap: 20px;
}
```

- `display`: Uses Flexbox to align the sub-sections (`flex`).
- `justify-content`: Distributes space between the sub-sections, placing space equally between them (`space-between`).
- `gap`: Adds 20 pixels of space between each sub-section, creating separation (`20px`).


```css
.intro-sub-section {
    flex: 1;
    padding: 20px;
    background-color: #2a2a2a;
    border-radius: 5px;
}
```

- `flex`: Allows each sub-section to take equal space within the flex container (`1`).
- `padding`: Adds 20 pixels of padding inside each sub-section, creating space around the content (`20px`).
- `background-color`: Sets the background color of the sub-sections to a slightly different shade of dark grey (`#2a2a2a`).
- `border-radius`: Rounds the corners of the sub-sections by 5 pixels, giving a softer, more visually appealing look (`5px`).


```css
.intro-sub-section h3 {
    font-size: 30px;
    margin-bottom: 10px;
}
```

- `font-size`: Sets the font size for the sub-section headings to 30 pixels.
- `margin-bottom`: Adds 10 pixels of space below the sub-section heading, providing separation from the content that follows.


```css
.intro-sub-section p {
    font-size: 14px;
    line-height: 1.6;
}
```

- `font-size`: Sets the font size for the sub-section paragraphs to 14 pixels.
- `line-height`: Sets the line height to 1.6 times the font size, ensuring better readability of the paragraph text.


```css
.intro-image {
    flex: 1;
    max-width: 40%;
    padding-left: 20px;
    padding-top: 80px;
}
```

- `flex`: Allows the image section to take up space within the flex container, but less than other flex items (`1`).
- `max-width`: Limits the maximum width of the image section to 40% of the container (`40%`).
- `padding-left`: Adds 20 pixels of space to the left of the image, creating separation between the text and the image (`20px`).
- `padding-top`: Adds 80 pixels of space above the image, positioning it lower within its container (`80px`).


```css
.intro-image img {
    width: 100%;
    height: auto;
    border-radius: 10px;
    border: 3px solid #333;
}
```

- `width`: Sets the image width to fill its container (`100%`).
- `height`: Adjusts the height automatically to maintain the image's original aspect ratio (`auto`).
- `border-radius`: Rounds the corners of the image by 10 pixels, giving it a softer appearance (`10px`).
- `border`: Adds a 3-pixel solid border around the image, with a color of dark grey (`#333`).


---
## Third Div
```html
<section class="about-me">
      <div class="about-images">
        <div class="about-image">
          <img src="" alt="Image 1" />
        </div>
        <div class="about-image">
          <img src="" alt="Image 2" />
        </div>
        <div class="about-image">
          <img src="" alt="Image 3" />
        </div>
      </div>
      <div class="about-content">
        <h2>About Me</h2>
        <div class="about-sub-sections">
          <div class="about-sub-section">
            <h3>My Vision</h3>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam, quis nostrud exercitation ullamco laboris
              nisi ut aliquip ex ea commodo consequat.
            </p>
          </div>
          <div class="about-sub-section">
            <h3>My Mission</h3>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam, quis nostrud exercitation ullamco laboris
              nisi ut aliquip ex ea commodo consequat.
            </p>
          </div>
        </div>
      </div>
    </section>
```


```css
.about-me {
    padding: 50px 80px;
    background-color: #202020;
    color: white;
}
```

- `padding`: Adds 50 pixels of padding to the top and bottom, and 80 pixels to the sides, providing space inside the element (`50px 80px`).
- `background-color`: Sets the background color of the `.about-me` section to dark grey (`#202020`).
- `color`: Sets the text color within the `.about-me` section to white.


```css
.about-images {
    display: flex;
    justify-content: space-between;
    margin-bottom: 40px;
}
```

- `display`: Uses Flexbox to align the images (`flex`).
- `justify-content`: Distributes space evenly between the images, placing space equally between them (`space-between`).
- `margin-bottom`: Adds 40 pixels of space below the images, creating separation from the text content that follows (`40px`).


```css
.about-image {
    flex: 1;
    margin: 0 10px;
}
```

- `flex`: Allows each image to take up equal space within the flex container (`1`).
- `margin`: Adds 10 pixels of horizontal space on both sides of each image, providing separation between images (`0 10px`).



```css
.about-image img {
    width: 100%;
    height: auto;
    border-radius: 10px;
    object-fit: cover;
}
```

- `width`: Sets the image width to fill its container (`100%`).
- `height`: Adjusts the height automatically to maintain the image's original aspect ratio (`auto`).
- `border-radius`: Rounds the corners of the images by 10 pixels, giving them a softer appearance (`10px`).
- `object-fit`: Ensures the images cover their container while maintaining their aspect ratio, cropping if necessary (`cover`).


```css
.about-content {
    text-align: center;
}
```

- `text-align`: Centers the text within the `.about-content` section (`center`).



```css
.about-content h2 {
    font-size: 55px;
    margin-bottom: 20px;
    position: relative;
}
```

- `font-size`: Sets the font size for the about heading to 55 pixels.
- `margin-bottom`: Adds 20 pixels of space below the heading, separating it from the content that follows.
- `position`: Sets the positioning of the heading to relative, which allows for additional styling, such as adding an underline or other elements relative to the heading.



```css
.about-content h2::after {
    content: '';
    display: block;
    width: 60px;
    height: 3px;
    background-color: white;
    margin: 10px auto;
}
```

- `content`: Creates an empty content block for the underline (`''`).
- `display`: Makes the pseudo-element a block element, allowing it to take up the full width specified (`block`).
- `width`: Sets the width of the underline to 60 pixels (`60px`).
- `height`: Sets the height of the underline to 3 pixels (`3px`).
- `background-color`: Sets the color of the underline to white.
- `margin`: Adds 10 pixels of space above and below the underline and centers it horizontally within the heading (`10px auto`).



```css
.about-sub-sections {
    display: flex;
    justify-content: center;
    gap: 50px;
}
```

- `display`: Uses Flexbox to align the sub-sections (`flex`).
- `justify-content`: Centers the sub-sections within the container (`center`).
- `gap`: Adds 50 pixels of space between each sub-section, creating separation (`50px`).



```css
.about-sub-section {
    flex: 1;
    max-width: 300px;
    text-align: left;
}
```

- `flex`: Allows each sub-section to take up equal space within the flex container (`1`).
- `max-width`: Limits the maximum width of each sub-section to 300 pixels, preventing them from becoming too wide (`300px`).
- `text-align`: Aligns the text within each sub-section to the left (`left`).




```css
.about-sub-section h3 {
    font-size: 30px;
    margin-bottom: 10px;
}
```

- `font-size`: Sets the font size for the sub-section headings to 30 pixels.
- `margin-bottom`: Adds 10 pixels of space below each sub-section heading, providing separation from the following content.



```css
.about-sub-section p {
    font-size: 14px;
    line-height: 1.6;
}
```

- `font-size`: Sets the font size for the sub-section paragraphs to 14 pixels.
- `line-height`: Sets the line height to 1.6 times the font size, ensuring better readability of the paragraph text.

## Fourth Div
```html
 <section class="my-vision">
      <div class="vision-content">
        <div class="vision-images">
          <div class="vision-image">
            <img src=" " alt="Vision Image 1" />
          </div>
          <div class="vision-image">
            <img src=" " alt="Vision Image 2" />
          </div>
        </div>
        <div class="vision-text">
          <h2>My Vision</h2>
          <div class="vision-item">
            <span class="vision-number">01.</span>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam, quis nostrud exercitation ullamco laboris
              nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in
              reprehenderit in voluptate velit
            </p>
          </div>
          <div class="vision-item">
            <span class="vision-number">02.</span>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam, quis nostrud exercitation ullamco laboris
              nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in
              reprehenderit in voluptate velit
            </p>
          </div>
        </div>
      </div>
    </section>
```



```css
.my-vision {
    padding: 50px 80px;
    background-color: #202020;
    color: white;
}
```

- `padding`: Adds 50 pixels of padding to the top and bottom, and 80 pixels to the sides, providing space inside the element (`50px 80px`).
- `background-color`: Sets the background color of the `.my-vision` section to dark grey (`#202020`).
- `color`: Sets the text color within the `.my-vision` section to white.



```css
.vision-content {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    gap: 20px;
}
```

- `display`: Uses Flexbox to align the vision content (`flex`).
- `justify-content`: Distributes space between the content elements, placing space equally between them (`space-between`).
- `align-items`: Aligns items to the top of the container (`flex-start`).
- `gap`: Adds 20 pixels of space between the images and text content, creating separation (`20px`).



```css
.vision-images {
    display: flex;
    gap: 20px;
    flex: 1;
    max-width: 50%;
}
```

- `display`: Uses Flexbox to align the images within the container (`flex`).
- `gap`: Adds 20 pixels of space between the two images, creating separation (`20px`).
- `flex`: Allows the images container to take up equal space within the flex layout (`1`).
- `max-width`: Limits the width of the images container to 50% of the section, preventing it from becoming too wide (`50%`).


```css
.vision-image {
    flex: 1;
}
```

- `flex`: Allows each image to take up equal space within the `.vision-images` flex container, ensuring all images are evenly distributed (`1`).



```css
.vision-image img {
    width: 100%;
    height: auto;
    border-radius: 10px;
    object-fit: cover;
    padding-top: 50px;
}
```

- `width`: Sets the image width to fill its container (`100%`).
- `height`: Adjusts the height automatically to maintain the image's original aspect ratio (`auto`).
- `border-radius`: Rounds the corners of the images by 10 pixels, giving them a softer appearance (`10px`).
- `object-fit`: Ensures the images cover their container while maintaining their aspect ratio, possibly cropping the image (`cover`).
- `padding-top`: Adds 50 pixels of space above the image, creating a visual separation from the content above (`50px`).



```css
.vision-text {
    flex: 1;
    padding-left: 20px;
}
```

- `flex`: Allows the text section to take up equal space within the `.vision-content` flex container (`1`).
- `padding-left`: Adds 20 pixels of space to the left of the text section, creating separation between the images and the text (`20px`).



```css
.vision-text h2 {
    font-size: 36px;
    margin-bottom: 20px;
    position: relative;
}
```

- `font-size`: Sets the font size for the vision heading to 36 pixels.
- `margin-bottom`: Adds 20 pixels of space below the heading, separating it from the content that follows.
- `position`: Sets the positioning of the heading to relative, which allows for additional styling, such as adding an underline or other elements relative to the heading.



```css
.vision-text h2::after {
    content: '';
    display: block;
    width: 60px;
    height: 3px;
    background-color: white;
    margin-top: 10px;
}
```

- `content`: Creates an empty content block for the underline (`''`).
- `display`: Makes the pseudo-element a block element, allowing it to take up the full width specified (`block`).
- `width`: Sets the width of the underline to 60 pixels (`60px`).
- `height`: Sets the height of the underline to 3 pixels (`3px`).
- `background-color`: Sets the color of the underline to white.
- `margin-top`: Adds 10 pixels of space above the underline, creating separation from the heading text (`10px`).




```css
.vision-item {
    display: flex;
    align-items: flex-start;
    margin-bottom: 20px;
}
```

- `display`: Uses Flexbox to align the vision items (`flex`).
- `align-items`: Aligns the items to the top of the container (`flex-start`).
- `margin-bottom`: Adds 20 pixels of space below each vision item, creating separation between consecutive items (`20px`).




```css
.vision-number {
    font-size: 24px;
    font-weight: bold;
    margin-right: 10px;
}
```

- `font-size`: Sets the font size for vision numbers to 24 pixels.
- `font-weight`: Makes the vision numbers bold.
- `margin-right`: Adds 10 pixels of space between the vision number and the accompanying text, creating separation (`10px`).


```css
.vision-item p {
    font-size: 14px;
    line-height: 1.6;
}
```

- `font-size`: Sets the font size for the vision item text to 14 pixels.
- `line-height`: Sets the line height to 1.6 times the font size, improving readability of the text.



---
## Fifth Div
```html
<section class="my-mission">
      <div class="mission-content">
        <div class="mission-text">
          <h2>My Mission</h2>
          <div class="mission-item">
            <span class="mission-number">01.</span>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam, quis nostrud exercitation ullamco laboris
              nisi ut aliquip ex ea commodo consequat.
            </p>
          </div>
          <div class="mission-item">
            <span class="mission-number">02.</span>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam, quis nostrud exercitation ullamco laboris
              nisi ut aliquip ex ea commodo consequat.
            </p>
          </div>
          <div class="mission-item">
            <span class="mission-number">03.</span>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam, quis nostrud exercitation ullamco laboris
              nisi ut aliquip ex ea commodo consequat.
            </p>
          </div>
          <div class="mission-item">
            <span class="mission-number">04.</span>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam, quis nostrud exercitation ullamco laboris
              nisi ut aliquip ex ea commodo consequat.
            </p>
          </div>
        </div>
        <div class="mission-images">
          <div class="mission-image">
            <div><img src=" " alt="Mission Image 1" /></div>
          </div>
          <div class="mission-image">
            <div><img src=" " alt="Mission Image 2" /></div>
          </div>
          <div class="mission-image">
            <div><img src=" " alt="Mission Image 3" /></div>
          </div>
          <div class="mission-image">
            <div><img src=" " alt="Mission Image 4" /></div>
          </div>
        </div>
      </div>
    </section>
```




```css
.my-mission {
    padding: 50px 80px;
    background-color: #202020;
    color: white;
}
```

- `padding`: Adds 50 pixels of padding to the top and bottom, and 80 pixels to the sides, providing space inside the element (`50px 80px`).
- `background-color`: Sets the background color of the `.my-mission` section to dark grey (`#202020`).
- `color`: Sets the text color within the `.my-mission` section to white.




```css
.mission-content {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    gap: 20px;
}
```

- `display`: Uses Flexbox to align the mission content (`flex`).
- `justify-content`: Distributes space between the content elements, placing space equally between them (`space-between`).
- `align-items`: Aligns items to the top of the container (`flex-start`).
- `gap`: Adds 20 pixels of space between the text and the image grid, creating separation (`20px`).




```css
.mission-text {
    flex: 1;
    padding-right: 20px;
}
```

- `flex`: Allows the text section to take up equal space within the `.mission-content` flex container (`1`).
- `padding-right`: Adds 20 pixels of space to the right of the text section, creating separation between the text and the image grid (`20px`).




```css
.mission-text h2 {
    font-size: 36px;
    margin-bottom: 20px;
    position: relative;
}
```

- `font-size`: Sets the font size for the mission heading to 36 pixels.
- `margin-bottom`: Adds 20 pixels of space below the heading, separating it from the content that follows.
- `position`: Sets the positioning of the heading to relative, which allows for additional styling, such as adding an underline or other elements relative to the heading.



```css
.mission-text h2::after {
    content: '';
    display: block;
    width: 60px;
    height: 3px;
    background-color: white;
    margin-top: 10px;
}
```

- `content`: Creates an empty content block for the underline (`''`).
- `display`: Makes the pseudo-element a block element, allowing it to take up the full width specified (`block`).
- `width`: Sets the width of the underline to 60 pixels (`60px`).
- `height`: Sets the height of the underline to 3 pixels (`3px`).
- `background-color`: Sets the color of the underline to white.
- `margin-top`: Adds 10 pixels of space above the underline, creating separation from the heading text (`10px`).



```css
.mission-item {
    display: flex;
    align-items: flex-start;
    margin-bottom: 20px;
}
```

- `display`: Uses Flexbox to align the mission items (`flex`).
- `align-items`: Aligns the items to the top of the container (`flex-start`).
- `margin-bottom`: Adds 20 pixels of space below each mission item, creating separation between consecutive items (`20px`).



```css
.mission-number {
    font-size: 24px;
    font-weight: bold;
    margin-right: 10px;
}
```

- `font-size`: Sets the font size for mission numbers to 24 pixels.
- `font-weight`: Makes the mission numbers bold.
- `margin-right`: Adds 10 pixels of space between the mission number and the accompanying text, creating separation (`10px`).




```css
.mission-item p {
    font-size: 14px;
    line-height: 1.6;
}
```

- `font-size`: Sets the font size for the mission item text to 14 pixels.
- `line-height`: Sets the line height to 1.6 times the font size, improving readability of the text.



```css
.mission-images {
    flex: 1;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 20px;
}
```

- `flex`: Allows the image grid to take up equal space within the `.mission-content` flex container (`1`).
- `display`: Uses CSS Grid layout to organize the images (`grid`).
- `grid-template-columns`: Creates a grid layout with 2 columns, each taking equal space (`repeat(2, 1fr)`).
- `gap`: Adds 20 pixels of space between the images, creating separation (`20px`).




```css
.mission-image div {
    overflow: hidden;
}
```

- `overflow`: Ensures that any content that overflows the container is hidden, which helps in keeping the image or any other content neatly inside its designated area (`hidden`).




```css
.mission-image img {
    width: 100%;
    height: auto;
    border-radius: 10px;
    object-fit: cover;
}
```

- `width`: Sets the image width to fill its container (`100%`).
- `height`: Adjusts the height automatically to maintain the image's original aspect ratio (`auto`).
- `border-radius`: Rounds the corners of the images by 10 pixels, giving them a softer appearance (`10px`).
- `object-fit`: Ensures the images cover their container while maintaining their aspect ratio, possibly cropping the image to fit (`cover`).




---
## Sixth Div
```html
<section class="technical-skills">
      <h2>My Technical Skills</h2>
      <div class="skills-content">
        <div class="skill-item">
          <div class="skill-image-wrapper">
            <img src="Sjg.jpeg" alt="Skill Image 1" />
          </div>
          <h3>Brigitte Schwartz</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim
          </p>
        </div>
        <div class="skill-item">
          <div class="skill-image-wrapper">
            <img src="Sjg.jpeg" alt="Skill Image 2" />
          </div>
          <h3>Alfredo Torres</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim
          </p>
        </div>
        <div class="skill-item">
          <div class="skill-image-wrapper">
            <img src="Sjg.jpeg" alt="Skill Image 3" />
          </div>
          <h3>Adora Montminy</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim
          </p>
        </div>
        <div class="skill-item">
          <div class="skill-image-wrapper">
            <img src="Sjg.jpeg" alt="Skill Image 4" />
          </div>
          <h3>Daniel Gallego</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim
          </p>
        </div>
      </div>
    </section>
```



```css
.technical-skills {
    padding: 50px 80px;
    background-color: #202020;
    color: white;
    text-align: center;
}
```

- `padding`: Adds 50 pixels of padding to the top and bottom, and 80 pixels to the sides, providing space inside the element (`50px 80px`).
- `background-color`: Sets the background color of the `.technical-skills` section to dark grey (`#202020`).
- `color`: Sets the text color within the `.technical-skills` section to white.
- `text-align`: Centers the heading and any other text within the `.technical-skills` section (`center`).



```css
.technical-skills h2 {
    font-size: 36px;
    margin-bottom: 40px;
    position: relative;
}
```

- `font-size`: Sets the font size for the skills heading to 36 pixels.
- `margin-bottom`: Adds 40 pixels of space below the heading, separating it from the content that follows.
- `position`: Sets the positioning of the heading to relative, which allows for additional styling, such as adding an underline or other elements relative to the heading.



```css
.technical-skills h2::after {
    content: '';
    display: block;
    width: 60px;
    height: 3px;
    background-color: white;
    margin: 10px auto;
}
```

- `content`: Creates an empty content block for the underline (`''`).
- `display`: Makes the pseudo-element a block element, allowing it to take up the full width specified (`block`).
- `width`: Sets the width of the underline to 60 pixels (`60px`).
- `height`: Sets the height of the underline to 3 pixels (`3px`).
- `background-color`: Sets the color of the underline to white.
- `margin`: Adds 10 pixels of space above and below the underline and centers it horizontally within the heading (`10px auto`).




```css
.skills-content {
    display: flex;
    justify-content: space-around;
    flex-wrap: nowrap;
    gap: 20px;
    overflow-x: auto;
}
```

- `display`: Uses Flexbox to align the skill items (`flex`).
- `justify-content`: Distributes space around the skill items, creating even spacing on all sides (`space-around`).
- `flex-wrap`: Prevents wrapping of the items, keeping them in a single row (`nowrap`).
- `gap`: Adds 20 pixels of space between each skill item (`20px`).
- `overflow-x`: Allows horizontal scrolling if the content overflows the container, ensuring all items remain accessible (`auto`).



```css
.skill-item {
    min-width: 20%;
    background-color: #252525;
    padding: 20px;
    border-radius: 10px;
    position: relative;
    text-align: center;
}
```

- `min-width`: Ensures each skill item takes up at least 20% of the container's width, providing a consistent size (`20%`).
- `background-color`: Sets the background color for each skill item to a darker grey (`#252525`).
- `padding`: Adds 20 pixels of padding inside each skill item, creating space around the content (`20px`).
- `border-radius`: Rounds the corners of each skill item by 10 pixels, giving a softer, more visually appealing look (`10px`).
- `position`: Allows for relative positioning within each skill item, enabling further positioning adjustments if needed (`relative`).
- `text-align`: Centers the text within each skill item (`center`).




```css
.skill-image-wrapper {
    overflow: hidden;
    border-radius: 10px;
    margin-bottom: 10px;
}
```

- `overflow`: Hides any content that overflows the boundaries of the image wrapper (`hidden`).
- `border-radius`: Rounds the corners of the images by 10 pixels, ensuring the images match the rounded look of their container (`10px`).
- `margin-bottom`: Adds 10 pixels of space below the image, creating separation from subsequent content (`10px`).



```css
.skill-image-wrapper img {
    width: 100%;
    height: auto;
    border-radius: 10px;
}
```

- `width`: Sets the image width to fill its container (`100%`).
- `height`: Adjusts the height automatically to maintain the image's original aspect ratio (`auto`).
- `border-radius`: Rounds the corners of the images by 10 pixels, giving them a softer appearance and ensuring consistency with the container's style (`10px`).



```css
.skill-item h3 {
    font-size: 18px;
    margin-bottom: 10px;
}
```

- `font-size`: Sets the font size for skill item headings to 18 pixels.
- `margin-bottom`: Adds 10 pixels of space below the heading, creating separation from the subsequent content (`10px`).



```css
.skill-item p {
    font-size: 14px;
    line-height: 1.6;
}
```

- `font-size`: Sets the font size for skill item paragraphs to 14 pixels.
- `line-height`: Sets the line height to 1.6 times the font size, improving readability of the paragraph text.

---
## Seventh Div

```html
<section class="portfolio-section">
      <div class="portfolio-content">
        <div class="portfolio-large-image">
          <img src="Sjg.jpeg" alt="Large Portfolio Image" />
        </div>
        <div class="portfolio-right-content">
          <div class="portfolio-small-image">
            <img src="Sjg.jpeg" alt="Small Portfolio Image" />
          </div>
          <div class="portfolio-text">
            <h2>My Portfolio</h2>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam, quis nostrud exercitation ullamco laboris
              nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in
              reprehenderit in voluptate velit.
            </p>
          </div>
        </div>
      </div>
    </section>
```


```css
.portfolio-section {
    padding: 50px 80px;
    background-color: #202020;
    color: white;
}
```

- `padding`: Adds 50 pixels of padding to the top and bottom, and 80 pixels to the sides, providing space inside the `.portfolio-section` (`50px 80px`).
- `background-color`: Sets the background color of the `.portfolio-section` to dark grey (`#202020`).
- `color`: Sets the text color within the `.portfolio-section` to white.




```css
.portfolio-content {
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
    gap: 20px;
}
```

- `display`: Uses Flexbox to align the portfolio content (`flex`).
- `align-items`: Aligns the items to the top of the container (`flex-start`).
- `justify-content`: Distributes space between the large image and the right content, ensuring they are spaced apart (`space-between`).
- `gap`: Adds 20 pixels of space between the large image and the right content, creating separation (`20px`).



```css
.portfolio-large-image {
    flex: 2;
}
```

- `flex`: Makes the large image container take up twice the space compared to other flex items, indicating it should be larger within the flex container (`2`).




```css
.portfolio-large-image img {
    width: 100%;
    height: auto;
    border-radius: 10px;
    object-fit: cover;
}
```

- `width`: Sets the large image width to fill its container (`100%`).
- `height`: Adjusts the height automatically to maintain the image's original aspect ratio (`auto`).
- `border-radius`: Rounds the corners of the large image by 10 pixels, giving it a softer appearance (`10px`).
- `object-fit`: Ensures the large image covers its container while maintaining its aspect ratio, cropping the image if necessary to fit (`cover`).


```css
.portfolio-right-content {
    display: flex;
    flex-direction: column;
    flex: 1;
    gap: 20px;
}
```

- `display`: Uses Flexbox to align the content of the right section (`flex`).
- `flex-direction`: Stacks the content vertically within the right section (`column`).
- `flex`: Allows this column to take up less space than the large image, making it smaller in comparison (`1`).
- `gap`: Adds 20 pixels of space between the small image and the text, providing separation (`20px`).




```css
.portfolio-small-image {
    flex: 1;
}
```

- `flex`: Allows the small image section to grow and fill available space within its flex container, ensuring it takes up an appropriate amount of space relative to other elements (`1`).




```css
.portfolio-small-image img {
    width: 100%;
    height: auto;
    border-radius: 10px;
    object-fit: cover;
}
```

- `width`: Sets the small image width to fill its container (`100%`).
- `height`: Adjusts the height automatically to maintain the image's original aspect ratio (`auto`).
- `border-radius`: Rounds the corners of the small image by 10 pixels, giving it a softer appearance (`10px`).
- `object-fit`: Ensures the small image covers its container while maintaining its aspect ratio, cropping the image if necessary to fit (`cover`).





```css
.portfolio-text {
    flex: 1;
}
```

- `flex`: Allows the text section to grow and fill available space within its flex container, ensuring it takes up an appropriate amount of space relative to other elements (`1`).



```css
.portfolio-text h2 {
    font-size: 36px;
    margin-bottom: 20px;
    position: relative;
}
```

- `font-size`: Sets the font size for the portfolio heading to 36 pixels.
- `margin-bottom`: Adds 20 pixels of space below the heading, separating it from the content that follows.
- `position`: Sets the positioning of the heading to relative, which allows for additional styling, such as adding an underline or other elements relative to the heading.



```css
.portfolio-text h2::after {
    content: '';
    display: block;
    width: 60px;
    height: 3px;
    background-color: white;
    margin-top: 10px;
}
```

- `content`: Creates an empty content block for the underline (`''`).
- `display`: Makes the pseudo-element a block element, allowing it to take up the full width specified (`block`).
- `width`: Sets the width of the underline to 60 pixels (`60px`).
- `height`: Sets the height of the underline to 3 pixels (`3px`).
- `background-color`: Sets the color of the underline to white.
- `margin-top`: Adds 10 pixels of space above the underline, creating separation from the heading text (`10px`).



```css
.portfolio-text p {
    font-size: 14px;
    line-height: 1.6;
}
```

- `font-size`: Sets the font size for the portfolio text to 14 pixels.
- `line-height`: Sets the line height to 1.6 times the font size, improving readability of the paragraph text.

---
## 8th Div

```html
 <section class="thank-you-section">
      <div class="thank-you-content">
        <div class="thank-you-text">
          <h2>Thank You</h2>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
            aliquip ex ea commodo consequat. Duis aute irure dolor in
            reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
            pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
            culpa qui officia deserunt mollit anim id est laborum.
          </p>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
            aliquip ex ea commodo consequat. Duis aute irure dolor in
            reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
            pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
            culpa qui officia deserunt mollit anim id est laborum.
          </p>
        </div>
        <div class="thank-you-image">
          <img src="Sjg.jpeg" alt="Thank You Image" />
        </div>
      </div>
    </section>
  </body>
</html>

```



```css
.thank-you-section {
    padding: 50px 80px;
    background-color: #202020;
    color: white;
}
```

- `padding`: Adds 50 pixels of padding to the top and bottom, and 80 pixels to the sides, providing space inside the `.thank-you-section` (`50px 80px`).
- `background-color`: Sets the background color of the `.thank-you-section` to dark grey (`#202020`).
- `color`: Sets the text color within the `.thank-you-section` to white.



```css
.thank-you-content {
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
    gap: 20px;
}
```

- `display`: Uses Flexbox to align the thank-you content (`flex`).
- `align-items`: Aligns the items to the top of the container (`flex-start`).
- `justify-content`: Distributes space between the text and image, ensuring they are spaced apart (`space-between`).
- `gap`: Adds 20 pixels of space between the text and image, creating separation (`20px`).




```css
.thank-you-text {
    flex: 1;
    max-width: 50%;
}
```

- `flex`: Allows the text section to grow and fill available space within its flex container, ensuring it takes up an appropriate amount of space relative to other elements (`1`).
- `max-width`: Limits the width of the text section to 50% of the `.thank-you-content`, preventing it from becoming too wide (`50%`).




```css
.thank-you-text h2 {
    font-size: 36px;
    margin-bottom: 20px;
    position: relative;
}
```

- `font-size`: Sets the font size for the thank-you heading to 36 pixels.
- `margin-bottom`: Adds 20 pixels of space below the heading, creating separation from the content that follows.
- `position`: Sets the positioning of the heading to relative, which allows for additional styling, such as adding an underline or other elements relative to the heading.




```css
.thank-you-text h2::after {
    content: '';
    display: block;
    width: 60px;
    height: 3px;
    background-color: white;
    margin-top: 10px;
}
```

- `content`: Creates an empty content block for the underline (`''`).
- `display`: Makes the pseudo-element a block element, allowing it to take up the full width specified (`block`).
- `width`: Sets the width of the underline to 60 pixels (`60px`).
- `height`: Sets the height of the underline to 3 pixels (`3px`).
- `background-color`: Sets the color of the underline to white.
- `margin-top`: Adds 10 pixels of space above the underline, creating separation from the heading text (`10px`).



```css
.thank-you-text p {
    font-size: 14px;
    line-height: 1.6;
    margin-bottom: 20px;
}
```

- `font-size`: Sets the font size for thank-you paragraphs to 14 pixels.
- `line-height`: Sets the line height to 1.6 times the font size, improving readability of the paragraph text.
- `margin-bottom`: Adds 20 pixels of space between paragraphs, providing separation and enhancing the layout's readability (`20px`).




```css
.thank-you-image {
    flex: 1.5;
}
```

- `flex`: Makes the image container take up 1.5 times the space of the text container within the flex layout, making it larger relative to the text (`1.5`).



```css
.thank-you-image img {
    width: 100%;
    height: auto;
    border-radius: 10px;
    object-fit: cover;
}
```

- `width`: Sets the image width to fill its container (`100%`).
- `height`: Adjusts the height automatically to maintain the image's original aspect ratio (`auto`).
- `border-radius`: Rounds the corners of the image by 10 pixels, giving it a softer appearance (`10px`).
- `object-fit`: Ensures the image covers its container while maintaining its aspect ratio, possibly cropping the image to fit (`cover`).






