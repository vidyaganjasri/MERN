# Explanation of the HTML Table

This is an example of an HTML **table** that shows a daily schedule.

## What Each Part Does

### `<table>`
- Starts the table.

### `<caption>`
- Adds a **title** above the table: *"My Daily Schedule"*

### `<thead>`, `<tbody>`, `<tfoot>`
- These are **semantic tags** used to organize the table:
  - **`<thead>`**: Table **header** section.
  - **`<tbody>`**: Main **body** of the table.
  - **`<tfoot>`**: Table **footer**.

---

## Table Rows and Columns

Each row is written using `<tr>` (table row), and inside it:

- `<th>` is for **header cells** (usually bold).
- `<td>` is for **data cells** (normal text).

---

## Special Attributes Used

- **`colspan="2"`**: One cell spans **two columns**.
- **`rowspan="2"`**: One cell spans **two rows**.
- **`&nbsp;`**: Adds a **blank space**.

---

## What the Table Shows

|         | Time           | Activity    |
|---------|----------------|-------------|
| Morning | 8am - 11am     | Write Code  |
| Break   | 12pm - 1pm     | Eat Lunch   |
| Afternoon | (spans 2 columns) | Yoga     |
| Evening | (spans 2 rows) 1pm - 5am | Free Time |
| Night   | —              | Sleep       |

### Footer Message:
> "And that's what I do every day, eat sleep and code"

---

This table is a structured and easy-to-read way of showing a **daily routine** using HTML.
