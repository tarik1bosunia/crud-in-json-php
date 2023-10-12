
# screenshots
<!-- ![Alt text](/posts/path/to/img.jpg "Optional title") -->
![home](./readme%20images/home.png "Home Page")

![update](./readme%20images/update_book1.png "Edit Book Page")

![new](./readme%20images/add_book2.png "Add New Book Page")

![add new book](./readme%20images/add_book1.png "Add New Book")

![update](./readme%20images/update_book2.png "Edit Book")
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

