---
layout: default
title: Creating the Frontend
nav_order: 2
permalink: /Example/Frontend
parent: An Example
has_children: false
---

# Creating our Frontend
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## **Photogallery Frontend**
### **HTML**
{% raw %}
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Photogallery</title>
    <link rel="stylesheet" href="/public/css/main.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Protest+Revolution&family=Protest+Riot&family=Sedan:ital@0;1&display=swap" rel="stylesheet">
    <script src="/public/js/main.js"></script>
</head>

<body>
    <div class="container">
        <div id="createImage">
            <h2>Create a New Image</h2>
            <form id="createForm">
                <input type="text" id="createImgTitle" placeholder="Title">
                <textarea id="createImgDescription" placeholder="Description" rows="4" cols="20"></textarea>
                <input type="text" id="createImgSrc" placeholder="Image Source URL">
                <input type="submit" class="submit" value="Create Image">
            </form>
        </div>
        
        <div id="imagesList">
            {% for img_id, img_data in images.items() %}
            <div class="imageForm">
                <figure data-img-id="{{ img_id }}">
                    <div class="pin"></div>
                    <img src="{{ img_data.src }}" alt="{{ img_data.title }}">
                    <figcaption>
                        <p>{{ img_data.title }}</p>
                        <p>{{ img_data.description }}</p>
                        <div class="buttons">
                            <button type="button" class="modifyBtn">Modify</button>
                            <button type="button" class="deleteBtn">Delete</button>
                        </div>
                    </figcaption>
                </figure>
            </div>
            {% endfor %}
        </div>
    </div>
</body>
</html>
```
{% endraw %}

#### **Document Setup**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Photogallery</title>

    <link rel="stylesheet" href="/public/css/main.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Protest+Revolution&family=Protest+Riot&family=Sedan:ital@0;1&display=swap" rel="stylesheet">

    <script src="/public/js/main.js"></script>
</head>
```

- **<!DOCTYPE html>**: Declares this document as an HTML5 document, which helps the browser to render it correctly.
- **<html lang="en">**: Opens the HTML document and specifies English as the primary language.
- **<head>**: Contains metadata about the HTML document.
- **&lt;meta charset="UTF-8"&gt;**: Sets the character encoding to UTF-8, which includes most characters from all known human languages.
- **&lt;title>Photogallery</title&gt;**: Sets the title of the webpage, which appears in the browser tab.
- The first <link> tag links the main CSS file, which contains styles for your webpage.
- The next two <link> tags establish a connection with Google Fonts, which is used to import custom fonts that are used on the webpage.
- The final <link> imports specific font styles from Google Fonts.
- **&lt;script&gt;**:Includes a JavaScript file that will make parts of the page interactive. This script is placed just before closing the <head> tag so that it's loaded early before the body content.

#### **Body**
```html
<body>
    <div class="container">
```

- **&lt;body&gt;**: Contains all the contents of the webpage that will be visible to the user.
- **&lt;div class="container"&gt;**: A div element used to wrap and style the central part of the webpage.

#### **Form for New Images**
```html
        <div id="createImage">
            <h2>Create a New Image</h2>
            <form id="createForm">
                <input type="text" id="createImgTitle" placeholder="Title">
                <textarea id="createImgDescription" placeholder="Description" rows="4" cols="20"></textarea>
                <input type="text" id="createImgSrc" placeholder="Image Source URL">
                <input type="submit" class="submit" value="Create Image">
            </form>
        </div>
```
- **&lt;div id="createImage"&gt;**: A division specifically for the image creation form.
- **&lt;h2&gt;Create a New Image&lt;/h2&gt;**: A heading that describes the purpose of the form.
- **&lt;form id="createForm"&gt;**: The form where users can input details for creating a new image.
- **&lt;input type="text"&gt;**: Text fields for entering the title and URL of the image.
- **&lt;textarea&gt;**: A larger text field for entering a description of the image.
- **&lt;input type="submit&gt;**: A button that submits the form data.

#### **Displaying the Images**
{% raw %}
```html
        <div id="imagesList">
            {% for img_id, img_data in images.items() %}
            <div class="imageForm">
                <figure data-img-id="{{ img_id }}">
                    <div class="pin"></div>
                    <img src="{{ img_data.src }}" alt="{{ img_data.title }}">
                    <figcaption>
                        <p>{{ img_data.title }}</p>
                        <p>{{ img_data.description }}</p>
                        <div class="buttons">
                            <button type="button" class="modifyBtn">Modify</button>
                            <button type="button" class="deleteBtn">Delete</button>
                        </div>
                    </figcaption>
                </figure>
            </div>
            {% endfor %}
        </div>
    </div>
</body>
</html>
```
{% endraw %}

- **&lt;div id="imagesList"&gt;**: Contains a dynamically generated list of images.
{% raw %} **{% for img_id, img_data in images.items() %}** {% endraw %}: A loop that iterates over each image data item passed from the backend.
- **&lt;figure&gt;**: Semantic HTML5 element used to represent self-contained content, often with an image.
- **&lt;img&gt;**: Displays the image.
- **&lt;figcaption&gt;**: Provides a caption or description for the content of the parent &lt;figure&gt;.
- **&lt;button&gt;**: Buttons for modifying and deleting the image.


### **CSS**
```css
body {
    background-image: url('../images/wood-background.jpg');
    width: 100%;
    font-family: 'Sedan', sans-serif;
    margin: 0;
}

.container {
    display: flex;
    flex-direction: row-reverse;
    justify-content: center;

    margin-top: 12.5%;
}

#imagesList {
    display: flex;
}

/* CARD CONTAINER */

figure {
    position: relative;
    width: 200px;
    height: 200px; /* Adjust the height as needed */
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    animation: sway 5s infinite alternate ease-in-out;
}

figure img {
    width: 100%;
    height: 100%;
    display: block;
    border: 5px solid white; /* Polaroid frame */
}

figcaption {
    text-align: center;
    padding: 5px;
    background-color: white;
    font-family: Arial, sans-serif;
    margin-left: 10px;
}

.pin {
    position: absolute;
    width: 20px;
    height: 20px;
    background-color: red;
    margin: 0 50%;
    border-radius: 50%;
    animation: none !important;
    border: 5px solid black;
  }

.imageForm .buttons {
    display: flex;
    justify-content: center;
    gap: 15px;
}


.buttons > button {
    padding: 2%;
}

.buttons > .modifyBtn {
    background-color: green;
}

.buttons > .deleteBtn {
    background-color: red;
}

@keyframes sway {
    0% { transform: rotate(-3deg); }
    100% { transform: rotate(3deg); }
}

/* CREATE CARD */

#createImage {
    background-color: white;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 0 5%;
    color: black;
}

#createImage form {
    display: flex;
    flex-direction: column;
    gap: 15px;
    align-items: center;
    width: 50%;
    padding-bottom: 15%;
}

#createImgTitle, #createImgDescription, #createImgSrc {
    padding: 7.5%;
}

.submit {
    padding: 10% 25%;
    border-radius: 15%;
    background-color: #e2e8f0;
}
```

#### **The Body**
```css
body {
    background-image: url('../images/wood-background.jpg');
    width: 100%;
    font-family: 'Sedan', sans-serif;
    margin: 0;
}
```
- Sets the background image, font, and other properties for the entire webpage.

#### **Styling for Image Cards**
```css
figure {
    position: relative;
    width: 200px;
    height: 200px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    animation: sway 5s infinite alternate ease-in-out;
}
```

- Styles the &lt;figure&gt; element to look like a card with dimensions, shadows, and a gentle swaying animation.

### **Javascript**
This part can be a bit confusing, so we're going to break it down. Don't get intimidated, we'll walk you through each step.

```js
document.addEventListener("DOMContentLoaded", function() {
  document.getElementById('createForm').addEventListener('submit', function(e) {
      e.preventDefault();
      const title = document.getElementById('createImgTitle').value;
      const description = document.getElementById('createImgDescription').value;
      const src = document.getElementById('createImgSrc').value;
      server_request('/images', { title, description, src }, 'POST', function(response) {
          window.location.reload();
      });
  });

  document.getElementById('imagesList').addEventListener('click', function(e) {
      const figure = e.target.closest('figure');
      if (!figure) return; 
      const imgId = figure.getAttribute('data-img-id');

      if (e.target.classList.contains('modifyBtn')) {
          const title = prompt("Enter new title:", figure.querySelector("figcaption > p").textContent);
          const description = prompt("Enter new description:", figure.querySelectorAll("figcaption > p")[1].textContent);
          const src = prompt("Enter new image source", figure.querySelector("img").src);

          server_request(`/images/${imgId}`, { title, description, src }, 'PUT', function(response) {
              window.location.reload();
          });
      } else if (e.target.classList.contains('deleteBtn')) {
          server_request(`/images/${imgId}`, {}, 'DELETE', function(response) {
              window.location.reload();
          });
      }
  });
});

function server_request(url, data={}, verb='GET', callback) {
  return fetch(url, {
      credentials: 'same-origin',
      method: verb,
      headers: {'Content-Type': 'application/json'},
      body: verb !== 'GET' ? JSON.stringify(data) : null,
  })
  .then(response => response.json())
  .then(response => {
      if(callback) callback(response);
  })
  .catch(error => console.error('Error:', error));
}
```

This code above does several things
1. Prevents a form from submitting the traditional way.
2. Handles adding a new image.
3. Allows users to modify or delete existing images.

#### **Setup**
```js
document.addEventListener("DOMContentLoaded", function() {
    ...
});
```

- This code waits until the entire webpage is loaded (all HTML is displayed, and all images or scripts are loaded). Only then does it start doing anything. Think of it like waiting for everyone to take their seats before starting a show.

#### **Form Submission**
```js
document.getElementById('createForm').addEventListener('submit', function(e) {
    e.preventDefault();
    ...
});
```

- This part looks for the form on the page where users enter information about a new image (like title, description, and where the image is located). Normally, when you submit a form, the page refreshes. e.preventDefault(); stops the page from refreshing because we want to do things our way without interrupting the user's experience.
- **getElementById('createForm')**: Finds the form on the page.
- **addEventListener('submit', ...)**: Adds a special listener to the form that activates when the form tries to submit.
- **e.preventDefault()**: Stops the form from submitting in the normal way (prevents the page from reloading).

#### **Handling Form Data**
```js
const title = document.getElementById('createImgTitle').value;
const description = document.getElementById('createImgDescription').value;
const src = document.getElementById('createImgSrc').value;
server_request('/images', { title, description, src }, 'POST', function(response) {
    window.location.reload();
});
```

- After stopping the form from doing its normal thing, we grab the data entered into the form fields (title, description, image source URL) and use it to make a request to our server to save this new image.
- **getElementById(...)**: Finds each input field by its ID and gets what the user has typed into .value.
- **server_request(...)**: This is a custom function (not shown here) that sends the data to the server.
- **window.location.reload()**: After the server says it's done, this command refreshes the page so the user can see the new image they added.

#### **Modifying or Deleting Images**
```js
document.getElementById('imagesList').addEventListener('click', function(e) {
    const figure = e.target.closest('figure');
    if (!figure) return; 
    ...
});
```

- This part handles clicks on either the "Modify" or "Delete" buttons for any image already listed on the page. It checks where the click happened and reacts only if it was on one of these buttons.
- **getElementById('imagesList')**: Finds the section of the page that lists all images.
- **e.target.closest('figure')**: Finds the closest figure element to where the click happened, which represents the image that the action is to be applied to.
- **if (!figure) return;**: Stops the function if the click wasn't on an image.

#### **Button Clicks**
```js
if (e.target.classList.contains('modifyBtn')) {
    ...
} else if (e.target.classList.contains('deleteBtn')) {
    ...
}
```

- If the "Modify" button is clicked, it asks the user to enter new details for the title, description, and source of the image. These new details are then sent to the server to update the image.
- If the "Delete" button is clicked, it tells the server to remove the image. No new data needs to be gathered; it just uses the image's ID to tell the server which image to delete.

[Previous: Design Process](Design Process){: .float-left .v-align-text-top}
[Next: Backend](Backend){: .float-right .v-align-text-top}
