<template>
    <div>
        <MDC :value="md" />
    </div>
</template>

<script setup lang="ts">
// will cause error in console
// Uncaught SyntaxError: The requested module '/_nuxt/node_modules/micromark/node_modules/debug/src/browser.js?v=a09048b5' 
// does not provide an export named 'default'
import { parseMarkdown } from '@nuxtjs/mdc/runtime'

const md = '```html\n<!DOCTYPE html>\n<html>\n<head>\n <meta charset="UTF-8">\n <title>Simple HTML Page</title>\n</head>\n<body>\n\n <h1>Hello, World!</h1>\n <p>This is a very simple HTML document.</p>\n <p>It has a heading and two paragraphs.</p>\n\n</body>\n</html>\n```\n\n### Explanation\n\nThis is a basic HTML document structure.\n\n1. `<!DOCTYPE html>`: This declaration defines the document type to be HTML5. It tells the browser what version of HTML to expect.\n2. `<html>`: This is the root element of an HTML page. All other elements are contained within this tag.\n3. `<head>`: This section contains meta-information about the HTML page. This information is not displayed directly on the page itself but is used by browsers, search engines, etc.\n * `<meta charset="UTF-8">`: This specifies the character encoding for the document, ensuring that text is displayed correctly across different browsers and operating systems. UTF-8 is the standard and recommended encoding.\n * `<title>`: This sets the title of the HTML page, which appears in the browser\'s title bar or tab.\n4. `<body>`: This section contains the visible content of the HTML page. Everything you see in the browser window (text, images, links, etc.) goes inside the `<body>` tag.\n * `<h1>`: This is a heading tag. `<h1>` is the largest and most important heading level. HTML provides heading levels from `<h1>` (largest) to `<h6>` (smallest).\n * `<p>`: This is a paragraph tag. It\'s used to define a block of text as a paragraph.\n\n**How to view it:**\n\n1. Copy the code above.\n2. Paste it into a plain text editor (like Notepad on Windows, TextEdit on Mac, or VS Code, Sublime Text, etc.).\n3. Save the file with an `.html` extension (e.g., `myfirstpage.html`).\n4. Open the saved file in a web browser (like Chrome, Firefox, Edge, Safari).\n\nYou will see a page with "Hello, World!" as a large heading, followed by two lines of text as paragraphs.'
</script>

<style scoped>

</style>