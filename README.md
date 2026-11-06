# Altfield landing page

A single static page served by GitHub Pages at https://altfield.io

It is one self-contained HTML file: the images are inlined as data URIs, so
there is nothing to configure on the host and the page loads in one request.
That matters more than usual here, because the product it sells is an SEO tool.

The page is generated from the app repository, which is private. Do not edit
`index.html` here by hand — edit `site/index.template.html` in that repo, run
`python3 site/build.py`, and copy `site/dist/index.html` over this one.

All transactions go through the Shopify App Store. This site takes no payments,
sets no cookies and collects no data.
