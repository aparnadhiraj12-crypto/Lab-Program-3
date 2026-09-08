# Lab Program 3 — Book Library Website

A small book-information website built two ways: a classic HTML **frameset** version
(the original assignment format) and a modern **dashboard** UI styled after a
reference design.

## Files

| File            | Purpose                                                                 |
|------------------|--------------------------------------------------------------------------|
| `index.html`     | Frameset page. Splits the window into two frames: `booklist.html` (left) and `bookinfo.html` (right). Open this file to view the site. |
| `booklist.html`  | Left frame. Renders a clickable list of book titles from `bookdata.js`. Each link loads that book's details into the right frame. |
| `bookinfo.html`  | Right frame. Reads the selected book's `id` from the URL query string and displays its cover color, author, year, genre, page count, and description. Shows a welcome message if no book is selected. |
| `bookdata.js`    | Shared dataset — a single `books` array (id, title, author, year, genre, pages, color, description) used by both `booklist.html` and `bookinfo.html`. Edit this file to add, remove, or update books. |
| `dashboard.html` | Standalone single-page dashboard UI ("Alcove") styled after a reference design — sidebar navigation, a "continue reading" card, and three book shelves (Currently reading / Next up / Finished). Independent of the frameset pages; open it directly in a browser. |
| `README.md`      | This file. |

## How to run

- **Frameset version:** open `index.html` in a browser.
- **Dashboard version:** open `dashboard.html` in a browser.

## Notes

- To add a book to the frameset version, add an entry to the `books` array in `bookdata.js` — both `booklist.html` and `bookinfo.html` pick it up automatically.
- To add books to the dashboard, edit the `data` object inside the `<script>` tag at the bottom of `dashboard.html`.
- The two versions currently use separate datasets/styles and are not linked to each other.