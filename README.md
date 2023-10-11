
<!-- ![Alt text](/posts/path/to/img.jpg "Optional title") -->
![home](./readme%20images/1.png "Home Page")
![new](./readme%20images/2.png "New  Page")
![update](./readme%20images/3.png "Edit Page")
# Tailwind Integration guide

### install & initialization tailwind css
```bash
npm install -D tailwindcss
npx tailwindcss init
```
### need to edit tailwind.config.js
```code
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./**/*.{php,html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

### add a 2 files file input.css & style.css
### in input.css write
```code
@tailwind base;
@tailwind components;
@tailwind utilities;
```

### link style.css file in index.php
```code
<link rel="stylesheet" href="style.css">
```

### run tailwind server
```bash
npx tailwindcss -i ./input.css -o ./style.css --watch
```

