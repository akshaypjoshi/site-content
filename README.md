# Site Content for akshayjoshi.dev

## Content
Writing, case studies and open-source cards come from Markdown in the public repo `akshaypjoshi/site-content` (configured in `lib/content.js`), fetched on the server and refreshed hourly:
- `writing/*.md` (also `blog/`, `notes/`): `title`, `date`, `summary`, `tags`, `draft`
- `work/*.md`: `title`, `industry`, `tags`, `image`, `order`. Any case studies here replace the built-in cards on the home page.
- `open-source/*.md`: `title`, `kind`, `url`, `order`

Sections with no content (Writing, Testimonials) are hidden. Add testimonials in the `quotes` array of `design-reference/Akshay Joshi.dc.html`. Set `GITHUB_TOKEN` on Vercel to avoid the unauthenticated GitHub API rate limit.
