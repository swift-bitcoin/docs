# Swift Bitcoin Docs

Generates DocC documentation from Swift Bitcoin's repo and deploy to `/docs` path of the organization's [website](https://swift-bitcoin.github.io/).

## Why separate repo?

Because it's easy to checkout Repo B (e.g. `swift-bitcoin` repo) from a GH Action running on Repo A (e.g. this repo) and later deploy to repo A's GH Pages. But it is not at all possible to run an action on Repo B and have it deploy artifacts another repo/org's GH pages.

Having a standalone docs repo with Pages will create the subfolder needed to host the documentation pages generated independently from the main site/blog.
