# open-in-minds

A tiny GitHub Pages "trampoline" that turns an `https://` link into a
`minds://create?git_url=...` deep link, so an **Open in Minds** button works
from places (like GitHub READMEs) that strip custom URL schemes.

## Usage

Link to:

```
https://boweiliu.github.io/open-in-minds/?git_url=<REPO_URL>[&branch=<BRANCH>]
```

The page reads `git_url` (and optional `branch`) from its own query string and
redirects to `minds://create?git_url=<REPO_URL>`. It also shows a manual
"Open in Minds" button and the raw deep link as a fallback, in case the browser
blocks the automatic launch or the Minds desktop app isn't installed.

Example (Local Print Bridge inspiration):

```
https://boweiliu.github.io/open-in-minds/?git_url=https://github.com/boweiliu/local-print-bridge
```

Static page only — no tracking, no server.
