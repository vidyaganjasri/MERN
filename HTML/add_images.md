# 📸 Image Embedding Guide Using HTML (For GitHub)

This document demonstrates how to use HTML inside Markdown files (like README.md) to embed images with more control such as size, captions, hover text, and lazy loading.

---

## 🖼️ Basic HTML Image with Size and Lazy Loading

```html
<img src="/images/ew.jpg" 
     alt="It's an animated cat which is disgusted" 
     width="200" 
     height="300" 
     loading="lazy">
```
- src: Path to the image.
- alt: Describes the image (helps with accessibility).
-width / height: Controls display size.
- loading="lazy": Improves page performance by loading the image only when it's near the viewport. 
  because if there are multiple images, then the browser might take some time to load all the images at once, 
  but that wouldn't be the case since this feature allows the images to only appear/ process when the user is viewing 
  the page it is installed, hence fast and effecient.
---

## ℹ️ What is loading="lazy"?
The loading="lazy" attribute delays loading of images until the user scrolls near them.

## ✅ Benefits:
- Faster initial load time

- Saves bandwidth (especially on mobile)

- Better performance on pages with many images

## 🖼️ Image with Tooltip
```html
<img src="images/wa.jpg" 
     alt="A mysterious image" 
     width="200" 
     height="350" 
     title="What is this? A man?">
```
title: Adds a tooltip when the user hovers over the image.

## 🖼️ Image with Caption Using `<figure>` and `<figcaption>`
```html
<figure>
    <img src="images/wa.jpg" 
         alt="Unknown content" 
         width="200" 
         height="350" 
         title="What is this? A man?">
    <figcaption>I don't remember what was in the image</figcaption>
</figure>
```
- <figure> groups the image and caption.

- <figcaption> provides a visible caption under the image.
