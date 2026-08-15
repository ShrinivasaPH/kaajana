# kaajana
kaajana


# Phase 1 done. Two files — put content.json next to index.html at the repo root.

Read this before you push, because there's one behaviour change that will look like a bug.

The page now fetches content.json, and browsers block fetch on the file:// protocol. Double-clicking index.html to preview locally will show the failure banner instead of the site. That's not broken — it's the security model. From now on, preview with:

# cd path/to/kaajana
# python3 -m http.server 8000