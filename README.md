# Markdown to HTML Renderer

This is a simple static web page designed to convert Markdown content from an `input.md` file into styled HTML, with code blocks highlighted by `highlight.js`.

## Features

*   **Single-file application**: All necessary HTML, CSS (via Tailwind CDN), and JavaScript (via Marked.js and Highlight.js CDNs) are contained within `index.html`.
*   **Responsive design**: Built with Tailwind CSS for a mobile-first, responsive layout.
*   **Markdown to HTML Conversion**: Utilizes `marked.js` to parse GitHub Flavored Markdown.
*   **Code Highlighting**: Integrates `highlight.js` to automatically detect and style code blocks.
*   **Easy Deployment**: Just place `index.html`, `input.md`, `README.md`, and `LICENSE` in any static web server and it works.

## How to Use

1.  **Clone or Download**: Get the `index.html`, `README.md`, and `LICENSE` files.
2.  **Create `input.md`**: In the same directory as `index.html`, create a file named `input.md`. This file will contain your Markdown content.
    *   **Example `input.md` content:**
        ```markdown
        # Welcome to My Markdown Page

        This is a paragraph of text. You can write your content here.

        ## Features

        *   Item 1
        *   Item 2
        *   Item 3

        ### Code Example

        ```javascript
        function helloWorld() {
            console.log("Hello, World!");
        }
        helloWorld();
        ```

        > This is a blockquote.

        **Bold text** and *italic text*.
        ```
3.  **Open `index.html`**: Simply open `index.html` in your web browser. The JavaScript within the page will automatically fetch `input.md`, convert its content, and display it.

## Project Structure

```
.
├── index.html
├── input.md   <- Your Markdown content goes here
├── README.md
└── LICENSE
```

## Technologies Used

*   [Tailwind CSS](https://tailwindcss.com/)
*   [Marked.js](https://marked.js.org/)
*   [Highlight.js](https://highlightjs.org/)
