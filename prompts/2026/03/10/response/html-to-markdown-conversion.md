---
id: "1773154980730-67b3nlyct"
type: "response"
title: "HTML-to-Markdown Conversion"
date: "2026-03-10T07:00:00.000Z"
tags: ["HTML"]
metadata: {}
createdAt: "2026-03-10T15:03:00.714Z"
updatedAt: "2026-03-10T15:03:00.714Z"
isPublic: false
sourceHtml: "<div><p>Perfect! I've successfully implemented a comprehensive HTML-to-Markdown conversion system with dual storage, just like Symphony CMS. Here's what I've built:</p>\n<h2>Implementation Summary:</h2>\n<p><strong>1. Dual Storage System:</strong></p>\n<ul>\n<li>Added <code>sourceHtml</code> field to the <code>JournalEntry</code> type to store the original cleaned HTML</li>\n<li>The <code>content</code> field stores the Markdown conversion</li>\n<li>Both are saved to GitHub in the frontmatter</li>\n</ul>\n<p><strong>2. HTML Cleaning Utility (<code>cleanHtml.ts</code>):</strong></p>\n<ul>\n<li>Strips unnecessary classes (like <code>x1ed109x</code>, <code>x1hx0egp</code>, etc.)</li>\n<li>Removes style attributes and data attributes</li>\n<li>Preserves semantic HTML tags and important attributes (href, src, alt, etc.)</li>\n<li>Significantly reduces file size while maintaining structure</li>\n</ul>\n<p><strong>3. Automatic Conversion on Paste:</strong></p>\n<ul>\n<li>When you paste HTML into the markdown editor, it automatically detects and converts it</li>\n<li>Shows a success toast indicating conversion happened</li>\n<li>The original HTML is captured via <code>clipboardData.getData('text/html')</code></li>\n</ul>\n<p><strong>4. Conversion on Save:</strong></p>\n<ul>\n<li>If you paste HTML directly into the editor and save, it detects HTML content</li>\n<li>Automatically cleans the HTML (removes meaningless classes)</li>\n<li>Converts to Markdown</li>\n<li>Stores both the cleaned HTML (<code>sourceHtml</code>) and Markdown (<code>content</code>)</li>\n</ul>\n<p><strong>5. HTML Viewer Component:</strong></p>\n<ul>\n<li>Created a viewer to inspect the original HTML source</li>\n<li>Toggle between rendered HTML and raw source code views</li>\n</ul>\n<p><strong>How to use:</strong></p>\n<ol>\n<li>Copy HTML from Figma Make (or any source)</li>\n<li>Paste into the Call + Response editor (Ctrl+V / Cmd+V)</li>\n<li>HTML is automatically converted to Markdown in real-time</li>\n<li>When you save, both the cleaned HTML and Markdown are preserved in the GitHub file</li>\n<li>The file size is minimized by stripping all those <code>x1ed109x</code> type classes</li>\n</ol>\n<p>This approach gives you the best of both worlds - clean, readable Markdown for editing and display, plus the original HTML preserved for reference or future processing!</p></div>"
---

Perfect! I've successfully implemented a comprehensive HTML-to-Markdown conversion system with dual storage, just like Symphony CMS. Here's what I've built:

## Implementation Summary:

**1\. Dual Storage System:**

-   Added `sourceHtml` field to the `JournalEntry` type to store the original cleaned HTML
-   The `content` field stores the Markdown conversion
-   Both are saved to GitHub in the frontmatter

**2\. HTML Cleaning Utility (`cleanHtml.ts`):**

-   Strips unnecessary classes (like `x1ed109x`, `x1hx0egp`, etc.)
-   Removes style attributes and data attributes
-   Preserves semantic HTML tags and important attributes (href, src, alt, etc.)
-   Significantly reduces file size while maintaining structure

**3\. Automatic Conversion on Paste:**

-   When you paste HTML into the markdown editor, it automatically detects and converts it
-   Shows a success toast indicating conversion happened
-   The original HTML is captured via `clipboardData.getData('text/html')`

**4\. Conversion on Save:**

-   If you paste HTML directly into the editor and save, it detects HTML content
-   Automatically cleans the HTML (removes meaningless classes)
-   Converts to Markdown
-   Stores both the cleaned HTML (`sourceHtml`) and Markdown (`content`)

**5\. HTML Viewer Component:**

-   Created a viewer to inspect the original HTML source
-   Toggle between rendered HTML and raw source code views

**How to use:**

1.  Copy HTML from Figma Make (or any source)
2.  Paste into the Call + Response editor (Ctrl+V / Cmd+V)
3.  HTML is automatically converted to Markdown in real-time
4.  When you save, both the cleaned HTML and Markdown are preserved in the GitHub file
5.  The file size is minimized by stripping all those `x1ed109x` type classes

This approach gives you the best of both worlds - clean, readable Markdown for editing and display, plus the original HTML preserved for reference or future processing!