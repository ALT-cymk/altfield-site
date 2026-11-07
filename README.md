# Altfield site

Static pages served by GitHub Pages at https://altfield.io

Generated from the app repository, which is private. Nothing here is edited by
hand: edit the templates in `site/` in that repo, run `python3 site/build.py`,
and copy the whole of `site/dist/` over this one — the page bodies, `assets/`,
`robots.txt`, `sitemap.xml`, `llms.txt` and `CNAME` are all build output.

The screenshots are real captures of the app, cut out of the App Store listing
images by `scripts/make-site-images.py`. They are ordinary files under
`assets/` rather than inlined data URIs, so a crawler can see them and a
browser can cache them between pages.

All transactions go through the Shopify App Store. This site takes no payments.

It carries HeyCatch analytics, installed from https://heycatch.ai/agents.md
and configured in `site/build.py`. The SDK autocaptures pageviews and clicks,
and sets a first-party cookie plus localStorage and sessionStorage entries
holding a device id, so the site is no longer cookie-free. There is no
consent banner in front of it.
