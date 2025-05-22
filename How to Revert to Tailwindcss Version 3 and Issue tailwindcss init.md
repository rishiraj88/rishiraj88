# How to Install Tailwind v3 to Work with `init` Command Again
Nowadays the version 4 of Tailwind CSS is common, and it is recommended as well. Still, if any of us desires to go down the rabbit hole  and experience the feel of Tailwindcss@3, this gist may be quite nice of a friend to make an Alice out of you:
- Install tailwindcss version 3 to use without `Vite`. Else you may install version 4+ to manage that with `Vite`:
<pre>npm install -D tailwindcss@3</pre>

- Initialize Tailwind (for version 3, not for v4+):
<pre>npx tailwindcss init</pre>

- Create a file named `styles.css` under src directory (you may have any other name for the file by your wish):
<pre>@tailwind base;
@tailwind components;
@tailwind utilities;</pre>

- In `tailwind.config.js`, set the scope of the files (directories and file extensions) to scan for CSS generation:
<pre>  content: ["*.{html}"],</pre>

- Generate the effective CSS declarations file (builtstyle.css here) with `npx tailwindcss`:
<pre>npx tailwindcss -i ./src/styles.css -o ./src/builtstyle.css --watch</pre>

- `-watch` here is optional. Apply it to avert issuing the generation of effective CSS declaration again and again manually. Elsewise define it as a script in package.json (or similar) file:
<pre>"scripts": {
    "start": "npx tailwindcss -i ./src/styles.css -o ./src/builtstyle.css && ng serve",
    "build": "npx tailwindcss -i ./src/styles.css -o ./src/builtstyle.css && ng build",
    "watch": "ng build --watch --configuration development",
},</pre>
