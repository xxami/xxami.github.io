## xxami.github.io
Zola based personal dev blog [[xxami.github.io](https://xxami.github.io/)]

## Requirements
- node.js / npx
- zola: https://www.getzola.org/

## Building
```sh
# build tailwind css (https://tailwindcss.com/)
# prefix with NODE_ENV=production to purge unused styles
npx tailwindcss-cli@latest build ./tailwind.css -o ./static/tailwind.css

# minify css (-comments '/LICENSE/' to preserve licensing)
npx clean-css-cli@latest static/tailwind.css -o static/tailwind.min.css

# test server (http://localhost:1111/)
zola serve
# build static site
zola build
```

## Theme resources
Custom theme mashup consisting of:
- Page macros & markup from [anpu-zola-theme](https://github.com/zbrox/anpu-zola-theme)
- Additional markup referenced from [dose](https://github.com/oltd/dose)
