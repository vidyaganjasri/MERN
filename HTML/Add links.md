# 🔗 HTML Anchor Tags & Semantic Elements

This file explains how to use the `<a>` anchor tag with different attributes and introduces key semantic elements like `<nav>`, `<section>`, and `<footer>`.

---

## 🔹 1. Anchor Tag (`<a>`)

The `<a>` tag is used to create hyperlinks in HTML.

### ✅ Examples:

```html
<a href="https://www.google.com/">click here to go to google.com</a>
<a href="about.html">About me</a>
```
href specifies the link destination.

You can link to external websites or internal pages.

---

## 🔹 2. Semantic HTML Elements
Semantic tags help describe the meaning of the content in a webpage.

Tag	Purpose
- <section>	Defines a section in the document
- <nav>	Navigation bar for links
- <footer>	Footer area (usually copyright info)
- <header>	Top section, usually contains logo/title

### ✅ Example:
html
```html
<section id="id_html"></section>
<nav></nav>
<a href="#">Back to top</a>
```
---

### ✅ Complete HTML Example

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>HTML Link & Semantic Elements Example</title>
</head>
<body>

  <!-- Top of the Page -->
  <header id="top">
    <h1>Welcome to My Website</h1>
    <p>This page demonstrates links and semantic elements.</p>
  </header>

  <!-- Navigation Bar -->
  <nav>
    <a href="#home">Home</a> |
    <a href="#about">About</a> |
    <a href="https://www.google.com/" target="_blank">Google</a> |
    <a href="about.html">About Page</a>
  </nav>

  <!-- Home Section -->
  <section id="home">
    <h2>Home</h2>
    <p>This is the home section of the website.</p>
    <a href="#top">Back to Top</a>
  </section>

  <!-- About Section -->
  <section id="about">
    <h2>About Me</h2>
    <p>I am learning HTML and web development!</p>
    <a href="#top">Back to Top</a>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2025 My Website</p>
  </footer>

</body>
</html>
```

---

# 🧠 Summary
- Use id attributes in sections for linking within the same page.

- Use semantic elements to improve structure and readability.

- Use target="_blank" to open links in a new tab.

- Use #top or #idName to jump to specific parts of the same page.

---

# 🔗 HTML Anchor Tags and Targets

This file explains how to use anchor (`<a>`) tags in HTML for downloading, opening links in new tabs, and navigating within a page.

---

## 📥 1. Downloading a File

You can allow users to download a file using the `download` attribute.

```html
<p>Download the image 
    <a href="ew.jpg" download>Cat face</a>
</p>
```
📝 When the user clicks "Cat face", the browser downloads the file ew.jpg.

---

## 🌐 2. Open in a New Tab
Use target="_blank" to open the link in a new tab.

```html
<p>
    Open <a href="https://www.google.com/" target="_blank">
        Google
    </a>
</p>
```
📝 Clicking this link will not replace the current page.

---

## 🔁 3. Open in the Same Tab
Use target="_self" or omit the target to open in the same tab.

``` html
<p>
    Open <a href="https://www.google.com/" target="_self">
        Google
    </a>
</p>
```
📝 This replaces the current page with the link destination.

---

## 🏠 4. Link to the Home Page
Use a forward slash / in href to return to the home (main) page of the site.

``` html
<p>
    <a href="/">Back to home</a>
</p>
```

📝 Works best in websites with defined routes or folder structures.

---

## 🔝 5. Link to the Top of the Page
Use href="#" to scroll back to the top of the current page.

```html
<p><a href="#">G.Srividya</a> </p>
```
📝 Good for “Back to top” links in long pages.

---

## ✅ Full Example
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <p>Download the image 
        <a href="ew.jpg" download>Cat face</a>
    </p>

    <p>
        Open <a href="https://www.google.com/" target="_blank">
            Google
        </a>
    </p>

    <p>
        Open <a href="https://www.google.com/" target="_self">
            Google
        </a>
    </p>

    <p>
        <a href="/">Back to home</a>
    </p>

    <p><a href="#">G.Srividya</a> </p>
</body>
</html>
```

