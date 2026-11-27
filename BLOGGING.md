# How to publish a blog post

Posts are plain Markdown files in the `_posts` folder. GitHub Pages turns them
into pages automatically, usually within a minute or two of saving.

## Publish from the GitHub website (no tools needed)

1. Open the repo on github.com and click **Add file → Create new file**.
2. In the name box, type `_posts/` and then a file name in the form
   `YYYY-MM-DD-short-title.md`, for example `_posts/2026-12-01-pricing-the-tail.md`.
   The date is the publish date; the short title becomes the web address.
3. Paste this at the top, then write the post below it in Markdown:

   ```
   ---
   title: "Pricing the tail"
   description: "One or two sentences for the blog list and link previews."
   tags: [Pricing, EVT]
   ---
   ```

4. Click **Commit changes**. The post appears on the Writing page, on the
   homepage ("Recent notes", latest three) and in the RSS feed.

`_drafts/example-post.md` shows the formatting you can use (headings, bold,
lists, links, quotes).

## Tips

- **Drafts:** files in `_drafts/` are never published. Keep work in progress
  there, and when it is ready, paste the text into a new file in `_posts/`.
- **Images:** in the repo, click **Add file → Upload files**, and type
  `images/` before the name (or drag in a folder called `images`). Then use
  `![Description](/images/file.png)` in the post.
- **Edit or unpublish:** open the file in `_posts` and edit it, or delete it.
- **Dates:** a post dated in the future is skipped. It won't appear on its own
  when the date arrives, because the site only rebuilds when something is
  committed, so date posts today or earlier.
- **If a post doesn't appear:** check the repo's **Actions** tab for a failed
  build. The usual causes are a missing `---` line, or a title or description
  with a colon or quote mark that isn't wrapped in double quotes.
