# 🧾 HTML Basics – Beginner & Interview Notes

## 📌 What is HTML?

- HTML stands for HyperText Markup Language.

- It is the standard language used to create and design web pages.

- HyperText: Links between web pages.

- Markup Language: Tags that describe how content is displayed.

📁 index.html
Default file expected by most web servers.

Always in lowercase, with no spaces in the filename.

🧱 Basic HTML Structure
html
Copy
Edit
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="author" content="Vidya">
    <meta name="description" content="This page contains all the things.">
    <title>My First Page</title>
    <link rel="stylesheet" href="main.css" type="text/css">
    <link rel="icon" href="img" type="image/x-icon">
  </head>
  <body>
    <h1>Welcome to My Web Page</h1>
    <p>This is a simple paragraph inside the body.</p>
  </body>
</html>
🧠 <head> – Metadata About the Page
Not visible on the actual webpage.

Stores information about the page.

✅ Examples:
html
Copy
Edit
<!-- Charset -->
<meta charset="UTF-8">

<!-- Author info -->
<meta name="author" content="Vidya">

<!-- Page description -->
<meta name="description" content="This page contains all the things.">

<!-- Page title -->
<title>HTML Basics</title>

<!-- Link to CSS file -->
<link rel="stylesheet" href="main.css" type="text/css">

<!-- Favicon -->
<link rel="icon" href="img" type="image/x-icon">
📄 <body> – Visible Content
This part contains what users see on the screen.

✅ Example:
html
Copy
Edit
<h1>Main Heading</h1>
<p>This is a paragraph that gives more details about the content.</p>
<h1> to <h6>: Headings (largest to smallest).

<p>: Paragraph text.

📌 Two Major Sections in HTML
Section	Purpose
<head>	Metadata and links (not displayed)
<body>	Visible page content

✅ HTML Validator
Check your HTML for correctness using the W3C Validator.


