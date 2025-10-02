# Ex.06 Book Front Cover Page Design
# Date:02.10.2025
# AIM:
To design a book front cover page using HTML and CSS.

# DESIGN STEPS:
## Step 1:
Create a Django Admin project.

## Step 2:
Create an app in the Django interface.

## Step 3:
Create a folder named 'static' in the app folder.

## Step 4:
Create a new HTML file in the static folder.

## Step 5:
Write the HTML code with relevant CSS properties.

## Step 6:
Choose the appropriate style and color scheme.

## Step 7:
Insert the images in their appropriate places.

## Step 8:
Publish the website in the LocalHost.

# PROGRAM:
book.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Book Cover - Web App Dev</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Open+Sans&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: #121212;
      font-family: 'Open Sans', sans-serif;
    }

    .book-cover {
      width: 500px;
      height: 720px;
      background: url("web2.png") no-repeat center center;
      background-size: cover;
      border-radius: 20px;
      position: relative;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.8);
      overflow: hidden;
      color: #fff;
    }

    .book-cover::before {
      content: "";
      position: absolute;
      inset: 0;
      background: rgba(0,0,0,0.5);
      border-radius: 20px;
      z-index: 0;
    }

    .book-cover > * {
      position: relative;
      z-index: 1;
      text-align: center;
    }

    .publisher {
      font-size: 18px;
      color: #ffcc00;
      font-weight: 700;
      margin-top: 25px;
      letter-spacing: 2px;
    }

    .title {
      font-family: 'Playfair Display', serif;
      font-size: 32px;
      font-weight: bold;
      margin: 25px 20px;
      line-height: 1.3;
      text-transform: uppercase;
      color: #00e6ff;
      text-shadow: 2px 2px 6px #000;
    }

    .subtitle {
      font-size: 16px;
      margin-bottom: 40px;
      font-style: italic;
      color: whitesmoke;
      text-shadow: 1px 1px 3px #000;
    }

    .footer {
      position: absolute;
      bottom: 30px;
      left: 30px;
      right: 30px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .footer .sec {
      font-weight: bold;
      font-size: 16px;
      color: #ffe600;
      text-shadow: 1px 1px 3px #000;
    }

    .footer-texts {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      gap: 5px;
    }

    .label {
      font-weight: bold;
      font-size: 14px;
      color: #66ff66;
      text-shadow: 1px 1px 3px black;
    }

    .author {
      font-size: 16px;
      font-weight: bold;
      color: #ffffff;
      text-shadow: 1px 1px 5px #000;
    }

    .author-photo {
      width: 90px;
      height: 90px;
      border-radius: 15px;
      border: 2px solid white;
      object-fit: cover;
      box-shadow: 0 0 15px rgba(255,255,255,0.6);
      transition: transform 0.3s ease;
    }

    .author-photo:hover {
      transform: scale(1.08);
    }
  </style>
</head>
<body>
  <div class="book-cover">
    <div class="publisher">SEC INSIGHTS</div>

    <div class="title">
      FUNDAMENTALS OF<br />
      WEB APPLICATION<br />
      DEVELOPMENT
    </div>

    <div class="subtitle">
      Deep Dive in HTML, CSS & JS Basics<br />
      Top seller of 2025
    </div>

    <!-- Footer Section -->
    <div class="footer">
      <div class="footer-texts">
        <div class="sec">SEC</div>
        <div class="label">SPECIAL EDITION</div>
        <div class="author">Dhivya Shree .R</div>
      </div>
      <img src="author.jpg" alt="Author" class="author-photo" />
    </div>
  </div>
</body>
</html>
```

# OUTPUT:
![output 1](<output 1.png>)


# RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
