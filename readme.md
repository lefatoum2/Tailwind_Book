## Installation via la CLI(Command Line Interface)

Installation de Nodejs(20.12.1) : https://nodejs.org/en/download/current

```
npm install -D tailwindcss
npx tailwindcess init
```


Si la dernière commande ne marche pas, créez vous même le fichier tailwind.config.js : 
```js
/** @type {import('tailwind').Config} */
module.exports = {
    content: ["./public/*.html"],
    theme: {
        extend : {},
    },
    plugins: [],
}
```
N'oubliez pas de créer le dossier public qui contiendra tous les pages html.
Créez un dossier "src", et le fichier input.css:
```js
@tailwind base;
@tailwind components;
@tailwind utilities;
```

 
```
npx tailwindcss -i ./src/input.css -o ./public/style.css
```
Cette commande va créer le fichier style.css de tailwind dans le dossier public.


