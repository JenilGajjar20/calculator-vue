# Calculator

This calculator is created using **Vue.js** along with **Tailwind CSS**.

## Project setup

### For Vue.js

- The CLI **(vue/@cli)** is a globally installed npm package and provides the vue command in your terminal.

```
npm install -g vue/@cli
```

- To create a vue project:

```
vue create <project-name>
```

### For Tailwind CSS

- Install **tailwindcss** using npm and create a **tailwind.config.js** file.

```
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init
```

- Create a **postcss.config.js** file and add below code:

```
module.exports = {
    plugins: {
        tailwindcss: {},
        autoprefixer: {}
    }
}
```

- Now add the path to the tailwind config file as show below:

```
module.exports = {
    content: ["./index.html", "./src/**/*.{vue, js, ts, jsx, tsx}"],
    theme: {
        extend: {}
    },
    plugins: []
}
```

- Create a **css** folder inside the assets folder and a **tailwind.css** file inside the css folder.

> Note: The assets folder is where you would put your **_images_** or **_stylesheets_** or **_videos_** etc. that you will import in the **main.js** file.

- Add the **@tailwind** directive to the file for each of the tailwind's layers.

```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

- Now import the css file in the **main.js** file.

```
import "./assets/css/tailwind.css";
```

- Run the server😀

```
npm run serve
```
