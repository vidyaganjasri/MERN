# 📰 HTML Content Elements – Explained with Code

## 📄 Web Pages Are Like Newspapers
- They contain **headings**, **subheadings**, and **paragraphs** (content).
- Structure helps with readability and hierarchy.

---

## 🏷️ Headings
- Headings range from **`<h1>` to `<h6>`**.
- `<h1>` is the **largest**, and `<h6>` is the **smallest**.
- They represent a **hierarchy of content**.

```html
<h1>Main Heading</h1>
<h2>Subheading</h2>
<h3>Smaller Subheading</h3>
```

## 🧱 Block-Level Elements vs Inline-Level Elements

### ✅ Block-Level Elements:
- Take up **full width**.
- Always start on a **new line**.
- Common examples:
  - `<h1>`
  - `<p>`
  - `<address>`

#### 🧪 Example:

```html
<p>This is a paragraph.</p>
<address>123 Web Street, HTML City</address>
```
### ✅ Inline-Level Elements:
- Flow within a line or paragraph.
- Do not start on a new line.

#### Common examples:

- <em>

- <strong>

- <abbr>

🧪 Example:
``` html
<p>This is <em>emphasized</em> and <strong>strongly emphasized</strong> text.</p>
<p>The term <abbr title="World Health Organization">WHO</abbr> is widely known.</p>
```

## ➖ Other Useful Tags

### `<hr>` – Horizontal Line
Adds a horizontal rule/line:

```html
<hr>
```

### `<br>` – Line Break  
Breaks the line:

```html
Line 1<br>
Line 2
```
### 💬 Comments in HTML
``` html
<!-- This is a comment -->
```
## 🔤 Special Characters (Entities)

| Symbol       | Code        | Output |
|--------------|-------------|--------|
| Space        | `&nbsp;`    |        |
| Less than    | `&lt;`      | <      |
| Greater than | `&gt;`      | >      |
| Copyright    | `&copy;`    | ©      |


```html
<p>5 &lt; 10 and 10 &gt; 5</p>
<p>&copy; 2025 My Website</p>
<p>This&nbsp;&nbsp;&nbsp;has&nbsp;extra&nbsp;spaces</p>
```
