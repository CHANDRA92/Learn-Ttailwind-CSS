# Tailwind Install guide
[Click](https://tailwindcss.com/docs/installation)

## 1. Install Tailwind CSS
Install <b>'tailwindcss'</b> via npm, and create your <b>'tailwind.config.js'</b> file.
```Terminal
npm install -D tailwindcss
npx tailwindcss init
```
## 2. Configure your template paths

Add the paths to all of your template files in your <b>'tailwind.config.js'</b> file.

```js
// change only the content (content:[])
  content: ["./src/**/*.{html,js}"],

```
## 3. Add the Tailwind directives to your CSS
Add the <b>'@tailwind'</b> directives for each of Tailwind’s layers to your main CSS file.
``` css
@tailwind base;
@tailwind components;
@tailwind utilities;
```
## 4. Start the Tailwind CLI build process
Run the CLI tool to scan your template files for classes and build your CSS.
```Terminal
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```
## 5. Start using Tailwind in your HTML
```html
    <link href="./output.css" rel="stylesheet">
```
