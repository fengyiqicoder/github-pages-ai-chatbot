# How to add an AI chatbot to a GitHub Pages site

A demo GitHub Pages site (a project page for a made-up library, `tidydate`) with an AI chatbot added by one script tag. No backend, no build step.

Live site: https://fengyiqicoder.github.io/github-pages-ai-chatbot/

## How it was added

1. Get a free key at [onetagai.com](https://onetagai.com) (1,000,000 free tokens, no card).
2. Paste this right before `</body>` in `index.html`, with your key:

```html
<script async src="https://onetagai.com/widget.js" data-key="YOUR_ONETAG_KEY"></script>
```

3. Commit. GitHub Pages redeploys in about a minute, and the chat button appears in the corner. It answers from the content of the page it is on.

If your site is built with Jekyll, put the tag in `_layouts/default.html` instead, so every page gets it.

The key in this repo is a public demo key with a small shared quota; use your own on your site. Guide: [Add AI to a GitHub Pages site](https://onetagai.com/guides/github-pages).
