## xxami.github.io
Zola based personal dev blog

## depends
- node.js / npx
- zola: https://www.getzola.org/

## building
```sh
# build tailwind css (https://tailwindcss.com/)
npx tailwindcss-cli@latest build ./tailwind.css -o ./static/tailwind.css
# prefix with NODE_ENV=production to purge unused styles
# minify css (-comments '/LICENSE/' to preserve licensing)
npx clean-css-cli@latest static/tailwind.css -o static/tailwind.min.css

# test server (http://localhost:1111/)
zola serve
# build static site
zola build
```
