
---
TODO: Introduction

## Starting Your Code

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Design Portfolio</title>
        <link rel="stylesheet" href="styles.css">
    </head>
    <body>
    </body>
</html>
```
---
## First Div of the Body

```html
<div class="container">
    <div class="text-section">
        <h1>Welcome to <br> My Design <br> Portfolio</h1>
        <button class="contact-button">Stellin John George / Graphic **Designer**</button>
    </div>
    <div class="image-section">
        <img src="Sjg.jpeg" alt="Stellin John George">
    </div>
</div>
```

```css
body {
    background-color: #000;
    color: #fff;
    font-family: 'Arial', sans-serif;
    margin: 0;
    padding: 0;
}
```
- `background-color`: Sets the background color of the page to black
- `color`: Sets the text color to white
- `font-family`: Sets the font style to Arial with a fallback to sans-serif
- `margin`: Removes default margin around the body
- `padding`: Removes default padding around the body

```css
.container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 80%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 50px;
    margin-bottom: 50px;
}
```
- `display`: Uses Flexbox to align child elements
- `justify-content`: Distributes space evenly between child elements
- `align-items`: Aligns items vertically in the center
- `width`: Sets the container width to 80% of the viewport
- `max-width`: Sets a maximum width for the container
- `margin`: Centers the container horizontally
- `padding`: Adds padding around the container
- `margin-bottom`: Adds space below the container to separate it from other sections

```css
.text-section {
    flex: 1;
    padding: 20px;
    text-align: left;
}

.text-section h1 {
    font-size: 64px;
    line-height: 1.2;
    margin: 0 0 20px 0;
}

.text-section p {
    font-size: 20px;
    line-height: 1.6;
    margin: 0 0 10px 0;
}
```
- `flex`: Allows the section to grow and fill available space
- `padding`: Adds padding inside the text section
- `text-align`: Aligns the text to the left
- `font-size`: Sets the font size for the heading to 64px
- `line-height`: Sets the line height to 1.2 times the font size
- `margin`: Removes top margin, adds 20px margin at the bottom
- `font-size`: Sets the font size for paragraphs to 20px
- `line-height`: Sets the line height to 1.6 times the font size
- `margin`: Removes top margin, adds 10px margin at the bottom

```css
.contact-button {
    background-color: #000;
    color: #fff;
    border: 1px solid #fff;
    padding: 15px 30px;
    margin-top: 30px;
    cursor: pointer;
    font-size: 20px;
    border-radius: 20px;
    text-align: center;
}
```
- `background-color`: Sets the button background color to black
- `color`: Sets the button text color to white
- `border`: Adds a white border around the button
- `padding`: Adds padding inside the button (top-bottom 15px, left-right 30px)
- `margin-top`: Adds a top margin of 30px
- `cursor`: Changes the cursor to a pointer when hovered over
- `font-size`: Sets the font size of the button text to 20px
- `border-radius`: Rounds the corners of the button
- `text-align`: Centers the text inside the button

---
## Second Div of the Body

```html
  <div class="container">
      <div class="text-section">
        <h1>Who is Stellin?</h1>
        <p>
          I'm a graphic designer with five years of experience. Today, I'm a
          full-time creative freelancer who loves to travel the world.
        </p>
        <div class="underline"></div>
      </div>
      <div class="image-section">
        <img src="Sjg.jpeg" alt="Person reading a book" />
      </div>
    </div>
```

```css
.underline {
    width: 60px;
    height: 2px;
    background-color: #fff;
    margin-top: 10px;
}
```
- `width`: Sets the width of the underline
- `height`: Sets the height of the underline
- `background-color`: Sets the underline color to white
- `margin-top`: Adds a top margin of 10px

```css
.image-section {
    flex: 1;
    display: flex;
    justify-content: center;
    align-items: center;
}
```
- `flex`: Allows the section to grow and fill available space
- `display`: Uses Flexbox to align child elements
- `justify-content`: Centers the child elements horizontally
- `align-items`: Centers the child elements vertically

```css
.image-section img {
    border-radius: 100%;
    width: 450px;
    height: 600px;
    object-fit: cover;
}
```
- `border-radius`: Makes the image fully rounded (elliptical shape)
- `width`: Sets the width of the image
- `height`: Sets the height of the image
- `object-fit`: Scales the image to cover the container while maintaining aspect ratio

---
## Third Div of the Body
```html
    <div class="background-section">
      <h1>My Background</h1>
      <div class="sub-section">
        <div class="sub-title"><span class="arrow">↳</span> Education</div>
        <ul>
          <li>MFA from the Ecole de Talens, 2019</li>
          <li>BFA from the Grover Wood Art Institute, 2018</li>
        </ul>
      </div>

      <div class="sub-section">
        <div class="sub-title">
          <span class="arrow">↳</span> Work Experience
        </div>
        <ul>
          <li>Freelance Graphic Designer and Illustrator, 2022-present</li>
          <li>Senior Graphic Designer at the Talens Institut, 2021-22</li>
          <li>Junior Creative at the NXTR Design Studio, 2020-21</li>
        </ul>
      </div>
    </div>
```
```css
.background-section {
    width: 80%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 50px;
}
```
- `width`: Sets the section width to 80% of the viewport
- `max-width`: Sets a maximum width for the section
- `margin`: Centers the section horizontally
- `padding`: Adds padding around the section

```css
.background-section h1 {
    font-size: 64px;
    margin-bottom: 30px;
}
```
- `font-size`: Sets the font size for the heading to 64px
- `margin-bottom`: Adds a bottom margin of 30px

```css
.sub-section {
    margin-top: 20px;
    padding-left: 40px;
}
```
- `margin-top`: Adds a top margin of 20px
- `padding-left`: Indents the section to the right by 40px

```css
.sub-title {
    font-size: 24px;
    display: flex;
    align-items: center;
    margin-bottom: 10px;
}
```
- `font-size`: Sets the font size for the sub-title to 24px
- `display`: Uses Flexbox to align items
- `align-items`: Centers the items vertically
- `margin-bottom`: Adds a bottom margin of 10px

```css
.arrow {
    font-size: 24px;
    margin-right: 10px;
}
```
- `font-size`: Sets the font size for the arrow icon
- `margin-right`: Adds a right margin of 10px

```css
ul {
    list-style-type: disc;
    padding-left: 20px;
    font-size: 18px;
    line-height: 1.6;
}
```
- `list-style-type`: Sets the list style to disc (bullet points)
- `padding-left`: Adds padding to the left of the list items
- `font-size`: Sets the font size for list items to 18px
- `line-height`: Sets the line height to 1.6 times the font size

---
## Fourth Div of the Body

```html
 <div class="art-section">
      <h1>My Art</h1>
      <div class="art-gallery">
        <div class="art-item">
          <img src="Sjg.jpeg" alt="Artwork 1" />
          <p>
            <span class="arrow">↳</span> Branding for Tost, a popular brunch
            spot in LA
          </p>
        </div>
        <div class="art-item">
          <img src="Sjg.jpeg" alt="Artwork 2" />
          <p>
            <span class="arrow">↳</span> Poster for La SSo, a bar in downtown
            NYC
          </p>
        </div>
        <div class="art-item">
          <img src="Sjg.jpeg" alt="Artwork 3" />
          <p><span class="arrow">↳</span> Poster for Des Lunes Film Society</p>
        </div>
      </div>
    </div>

```

```css
.art-section h1 {
    margin-bottom: 30px;
    padding-left: 350px;
    font-size: 64px;
}
```
- `margin-bottom`: Adds a bottom margin of 30px
- `padding-left`: Indents the heading to the right by 350px
- `font-size`: Sets the font size for the heading to 64px

```css
.art-gallery {
    display: flex;
    justify-content: space-between;
    gap: 0px;
    padding: 100px 190px;
}
```
- `display`: Uses Flexbox to align child elements
- `justify-content`: Distributes space evenly between child elements
- `gap`: Sets the space between gallery items to 0
- `padding`: Adds padding inside the gallery (top-bottom 100px, left-right 190px)

```css
.art-item {
    text-align: center;
    flex: 1;
}
```
- `text-align`: Centers the text inside the item
- `flex`: Allows the item to grow and fill available space

```css
.art-item img {
    width: 300px;
    height: 300px;
    border-radius: 20px 20px 0 0;
    object-fit: cover;
    margin-bottom: 10px;
}
```
- `width`: Sets the width of the image
- `height`: Sets the height of the image
- `border-radius`: Rounds the top corners of the image
- `object-fit`: Scales the image to cover the container while maintaining aspect ratio
- `margin-bottom`: Adds a bottom margin of 10px

```css
.art-item p {
    font-size: 18px;
    line-height: 1.6;
    margin-top: 10px;
}
```
- `font-size`: Sets the font size for the paragraph
- `line-height`: Sets the line height to 1.6 times the font size
- `margin-top`: Adds a top margin of 10px

---
## Fifth Div of the Body

```html
    <div class="quote-section">
      <div class="quote-text">
        <h1>Art speaks where words are unable to explain.</h1>
      </div>
      <div class="quote-image">
        <img src="Sjg.jpeg" alt="Person reading a book" />
      </div>
    </div>
```

```css
.quote-section {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 80%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 50px;
}
```
- `display`: Uses Flexbox to align child elements
- `justify-content`: Distributes space evenly between child elements
- `align-items`: Aligns items vertically in the center
- `width`: Sets the section width to 80% of the viewport
- `max-width`: Sets a maximum width for the section
- `margin`: Centers the section horizontally
- `padding`: Adds padding around the section

```css
.quote-text {
    flex: 1;
    text-align: left;
    padding-right: 30px;
}
```
- `flex`: Allows the section to grow and fill available space
- `text-align`: Aligns the text to the left
- `padding-right`: Adds padding to the right

```css
.quote-text h1 {
    font-size: 64px;
    line-height: 1.2;
    margin: 0;
}
```
- `font-size`: Sets the font size for the quote text
- `line-height`: Sets the line height to 1.2 times the font size
- `margin`: Removes default margin

```css
.quote-image {
    flex: 1;
    display: flex;
    justify-content: center;
    align-items: center;
}
```
- `flex`: Allows the section to grow and fill available space
- `display`: Uses Flexbox to align child elements
- `justify-content`: Centers the child elements horizontally
- `align-items`: Centers the child elements vertically

```css
.quote-image img {
    width: 400px;
    height: 600px;
    border-radius: 50% / 50%;
    object-fit: cover;
    transform: rotate(-90deg);
}
```
- `width`: Sets the width of the image
- `height`: Sets the height of the image
- `border-radius`: Makes the image elliptical
- `object-fit`: Scales the image to cover the container while maintaining aspect ratio
- `transform`: Rotates the image by -90 degrees

---
## Sixth Div of the Body

```html
    <div class="work-section">
      <h1>More of My Work</h1>
      <div class="work-gallery">
        <div class="work-item">
          <img src="Sjg.jpeg" alt="Artwork 1" />
          <p><span class="arrow">↳</span> My personal artwork</p>
        </div>
        <div class="work-item">
          <img src="Sjg.jpeg" alt="Artwork 2" />
          <p><span class="arrow">↳</span> Neon sign for Fattys Bar</p>
        </div>
        <div class="work-item">
          <img src="Sjg.jpeg" alt="Artwork 3" />
          <p><span class="arrow">↳</span> Sign for San Diego Apparel</p>
        </div>
        <div class="work-item">
          <img src="Sjg.jpeg" alt="Artwork 4" />
          <p><span class="arrow">↳</span> Neon sign for Jeff's</p>
        </div>
      </div>
    </div>
```

```css
.work-section {
    width: 80%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 50px;
    text-align: left;
}
```
- `width`: Sets the section width to 80% of the viewport
- `max-width`: Sets a maximum width for the section
- `margin`: Centers the section horizontally
- `padding`: Adds padding around the section
- `text-align`: Aligns the text to the left

```css
.work-section h1 {
    font-size: 64px;
    margin-bottom: 30px;
}
```
- `font-size`: Sets the font size for the heading to 64px
- `margin-bottom`: Adds a bottom margin of 30px

```css
.work-gallery {
    display: flex;
    justify-content: space-between;
    gap: 20px;
}
```
- `display`: Uses Flexbox to align child elements
- `justify-content`: Distributes space evenly between child elements
- `gap`: Adds 20px space between gallery items

```css
.work-item {
    text-align: center;
    flex: 1;
}
```
- `text-align`: Centers the text inside the item
- `flex`: Allows the item to grow and fill available space

```css
.work-item img {
    width: 250px;
    height: 300px;
    border-radius: 50% 50% 0 0;
    object-fit: cover;
    margin-bottom: 10px;
}
```
- `width`: Sets the width of the image
- `height`: Sets the height of the image
- `border-radius`: Rounds the top corners of the image
- `object-fit`: Scales the image to cover the container while maintaining aspect rat*/
- `margin-bottom`: Adds a bottom margin of 10px

```css
.work-item p {
    font-size: 18px;
    line-height: 1.6;
    margin-top: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
}
```
- `font-size`: Sets the font size for the paragraph
- `line-height`: Sets the line height to 1.6 times the font size
- `margin-top`: Adds a top margin of 10px
- `display`: Uses Flexbox to align items
- `align-items`: Centers the items vertically
- `justify-content`: Centers the items horizontally

---
## Seventh Div of the Body

```html
   <div class="contact-section">
      <h1>Reach Out to Me</h1>
      <div class="contact-details">
        <div class="contact-item">
          <h2>Address</h2>
          <p>123 Anywhere St., Any City<br />State, Country 12345</p>
        </div>
        <div class="contact-item">
          <h2>Email</h2>
          <p>hello@reallygreatsite.com</p>
        </div>
        <div class="contact-item">
          <h2>Phone</h2>
          <p>(123) 456 7890</p>
        </div>
      </div>
      <div class="collaborate">
        <p><span class="arrow">↳</span> Let's collaborate</p>
      </div>
    </div>
  </body>
</html>

```

```css
.contact-section {
    width: 80%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 50px;
    text-align: left;
}
```
- `width`: Sets the section width to 80% of the viewport
- `max-width`: Sets a maximum width for the section
- `margin`: Centers the section horizontally
- `padding`: Adds padding around the section
- `text-align`: Aligns the text to the left

```css
.contact-section h1 {
    font-size: 64px;
    margin-bottom: 30px;
}
```
- `font-size`: Sets the font size for the section title
- `margin-bottom`: Adds a bottom margin of 30px

```css
.contact-details {
    display: flex;
    justify-content: space-between;
    margin-bottom: 50px;
}
```
- `display`: Uses Flexbox to align child elements
- `justify-content`: Distributes space evenly between child elements
- `margin-bottom`: Adds space between contact details and the collaborate call


```css
.contact-item h2 {
    font-size: 24px;
    margin-bottom: 10px;
}
```
- `font-size`: Sets the font size for the sub-heading
- `margin-bottom`: Adds a bottom margin of 10px

```css
.contact-item p {
    font-size: 18px;
    line-height: 1.6;
}
```
- `font-size`: Sets the font size for the paragraph
- `line-height`: Sets the line height to 1.6 times the font size
```css
.collaborate {
    text-align: left;
}
```
`text-align`: Aligns the text to the left
```css
.collaborate p {
    font-size: 18px;
    display: flex;
    align-items: center;
}
```
- `font-size`: Sets the font size for the paragraph
- `display`: Uses Flexbox to align items
- `align-items`: Centers the items vertically
```css
.arrow {
    font-size: 24px;
    margin-right: 10px;
}
```
- `font-size`: Sets the font size for the arrow icon
- `margin-right`: Adds a right margin of 10px