To reproduce gatsby issue [#25207](https://github.com/disintegrator/gatsby-25207):

- Clone this repo
- Run `npm install && npm run build`
- Open `public/index.html`
  - Look for references to icons added by gatsby-plugin manifest: `rel="icon"` and `rel="apple-touch-icon"`
  - Note the fully qualified and expected URLs
- Open `public/manifest.webmanifest`
  - Note the icon URLs only contain `pathPrefix` and not `assetPrefix`
