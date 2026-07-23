# pepita starters

Seed content that pepita fetches **one file at a time** at content-creation time,
via the GitHub Contents API (single-file reads, not repo-generate).

Each starter is a plain file addressed by path. Editing a file here changes the
seed for the next artifact of that kind; existing artifacts are unaffected.

| Path | Used for |
|------|----------|
| `form-email-confirmation.html` | The body of a new confirmation-email template (editor - Files - Templates). |

The app KV-caches each file for ~1h and falls back to a bundled copy if the
fetch fails, so nothing here is load-bearing for availability.