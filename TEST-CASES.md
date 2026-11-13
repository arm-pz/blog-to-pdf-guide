# Test cases: blog-to-pdf-guide

## Executed (2026-11-13)

Claude Code 2.1.323, skill installed in a fresh project next to other skills (docx, pptx, xlsx, pdf, design, searchfit-seo, remotion), each prompt sent with `claude -p` in a new session; first Skill call recorded.

| Prompt | Expected | Loaded | Result |
| --- | --- | --- | --- |
| Turn my blog posts into an ebook I can give away. | should load | blog-to-pdf-guide | pass |
| I want something to give people for joining my email list, I've written loads of posts on sourdough. | should load | blog-to-pdf-guide | pass |
| Compile these 6 articles into a free guide for my newsletter signup. | should load | blog-to-pdf-guide | pass |
| Merge these three PDFs into one file. | should not load | anthropic-skills:pdf | pass |

**4 pass, 0 fail.**

## Reviewed only (read from descriptions, not executed)

| # | Type | Message | Expected | Result |
|---|---|---|---|---|
| 1 | C | "Turn my blog posts into an ebook" | blog-to-pdf-guide | pass |
| 2 | C | "Make a lead magnet from these 6 articles" | blog-to-pdf-guide | pass |
| 3 | C | "Compile these posts into a free guide for my newsletter signup" | blog-to-pdf-guide | pass |
| 4 | I | "I want something to give people for joining my email list, I've written loads of posts" | blog-to-pdf-guide | pass |
| 5 | I | "Repackage my Substack archive into one downloadable" | blog-to-pdf-guide | pass |
| 6 | N | "Merge these three PDFs" | pdf | pass |
| 7 | N | "Write a new blog post about SEO" | searchfit-seo:create-content | pass |
| 8 | N | "Make my posts rank better" | searchfit-seo | pass |
