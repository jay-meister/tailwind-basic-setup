### TailwindCSS setup

```sh
npm i tailwindcss -s
mkdir src && touch src/style.css
mkdir dist && touch dist/index.html dist/style.css

# only necessary for custom config:
npx run tailwind init
# or 
npx run tailwind init --full
```

src/style.css
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

package.json
```json
"scripts": {"build:css": "tailwind build src/style.css -o dist/style.css"}
```

```sh
npm run build:css
```


### Useful VS Code packages
Tailwind CSS IntelliSense - bradlc.vscode-tailwindcss
Live Server
  - Live serve static HTML
HTML CSS Support - ecmel.vscode-html-css
  - Autofill for available css classes

### Youtube link: 
https://www.youtube.com/watch?v=UBOj6rqRUME&ab_channel=TraversyMedia