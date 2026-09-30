# Bled Heritage / Qashabia Messaad — Public Store

Static catalog website. No checkout, cart or payment.

## Content source

The local `bled-admin` app publishes content to the same GitHub repository. The store reads:

```text
products/index.json
products/<slug>/product.json
content/store.json
content/home.json
content/categories.json
content/brand/*
content/images/*
```

Do not edit published content manually if you are using Admin.

## Local preview

Because the site loads JSON with `fetch()`, serve it through a local HTTP server instead of opening `index.html` directly.

Example:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## GitHub Pages

Publish this folder as the public site. Before launch, replace the placeholder sitemap domain in `sitemap.xml` with the final domain and add the real store information through Admin.
