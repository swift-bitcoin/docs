# Swift Bitcoin Docs

Generates DocC documentation from Swift Bitcoin's repo and deploy to [/docs](https://swift-bitcoin.github.io/docs/documentation/bitcoin) path of the organization's website.

## Why separate repo?

Because it's simple enough to checkout Repo B (e.g. `swift-bitcoin` repo) from a GitHub Action running on Repo A (e.g. this repo) and deploy the generated docs to Repo A's GitHub Pages URL while it is not at all possible to run an Action directly on Repo B and have it deploy the docs artifacts to a different repo's Pages URL (or to the organization's Pages URL).

Having a standalone docs repo with Pages on will also create the subfolder needed (in this case _docs_) to host the documentation pages generated independently from the main site and blog.
