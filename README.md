

## When Live Sass Compilation Has Issues

1. Compile Sass using:

```bash
sass ./css/main.scss ./css/main.css
```

2. For watching changes and generating a source map, use:

```bash
sass --watch ./css/main.scss:./css/main.css --source-map
```

## Compiling SASS
3. node -v 
4. npm init
5. 
```bash
npm install gulp gulp-sass sass --save-dev
```


### Compiling sass with gulp

link :(https://www.youtube.com/watch?v=Sk5jMurFHCo&list=PL4cUxeGkcC9jxJX7vojNVK-o8ubDZEcNb&index=2)

<hr>

- If your SCSS is not compiling into CSS, here are a few potential reasons and steps to troubleshoot:

File Paths: Make sure the SCSS file path is correct. For example, if you're running this command:

bash
Copy code
sass ./css/test.scss ./css/test.css
Verify that the file test.scss exists in the css folder and the output path is also correct.

Live Sass Compiler: If you're using a live Sass compiler (like the VS Code extension), ensure that it is activated and monitoring the correct folder. Make sure you have a .scss file with proper syntax.

Syntax Issues: Double-check your SCSS for syntax errors. In your provided code, the SCSS looks fine, but missing semicolons or incorrect nesting could prevent proper compilation.

Google Fonts Import: Your import for Google Fonts is correct:

scss
Copy code
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;600;700;800;900&display=swap');
However, check that you have network access for the font to be loaded correctly. Fonts may not impact SCSS compilation, but make sure it's not blocked.

Sass Installation: Ensure that Sass is installed correctly by running:

bash
Copy code
sass --version
If this fails, you may need to install it:

bash
Copy code
npm install -g sass
SCSS Watch Command: Use the watch command to continuously compile SCSS to CSS:

bash
Copy code
sass --watch ./css/test.scss ./css/test.css
This will automatically compile whenever changes are detected.

