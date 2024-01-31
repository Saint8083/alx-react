0x00. Webpack
=============
Learning Objectives
-------------------
-   How to setup Webpack for a basic project
-   Entry points, output, and loaders
-   How to add plugins
-   How to split your code into chunks
-   How to setup a dev server
Resources
---------
**Read or watch**:
-   [Webpack documentation](https://alx-intranet.hbtn.io/rltoken/XEFTUAcZ_9sKurp1Bui7ug "Webpack documentation")
-   [Webpack beginner guide](https://alx-intranet.hbtn.io/rltoken/6ngQzrV7xeKJjcRwdmrYAQ "Webpack beginner guide")
-   [npm-package.json](https://alx-intranet.hbtn.io/rltoken/P00rJM5qCeaf33hsPuhgog "npm-package.json")


Tasks
-----

	@@ -136,7 +135,6 @@ Create a specific configuration for Webpack.
-   Directory: `0x00-Webpack`
-   File: `task_2/package.json, task_2/css/main.css, task_2/webpack.config.js, task_2/js/dashboard_main.js, task_2/public/index.html`

 Done? Help Check your code

### 3\. Dev servers, modules, and tree shaking

mandatory
Using the folder named `task_3`. **Set up a development server:**
-   Reuse the code from `task_2`.
-   Modify the Webpack config to setup a development server running on the port 8564.
-   Modify the Webpack config to set its `mode` to `development`.
-   Add a script in the `package.json` to start the server and open the browser with `npm run start-dev`.
**Divide the code into modules:**
-   Divide the main bundle into three modules.
-   `header` should contain a `header.css` and `header.js` files.
-   Import jQuery, and add the logo and the H1 title to the `header.js` file (with content `Holberton Dashboard`). Add a console.log printing `Init header`.
-   Add the needed style to the `header.css` file.
-   `body` should contain a `body.css` and `body.js` files.
-   Import jQuery, Lodash and add the body code (button, counter) in the `body.js` file.
-   Add the needed style to the `body.css` file.
-   `footer` should contain a `footer.css` and `footer.js` files.
-   Import jQuery, and append a paragraph the copyright text `Copyright - Holberton School`.
-   Add the needed style to the `footer.css` file.
-   Modify the Webpack configuration to support three different entry points (`header`, `body`, `footer`). Each entry point should generate a filename with the following format `name_of_the_file.bundle.js`.
-   Do NOT have a `task_3/public/` directory pushed to your repository.
-   Add a plugin to Webpack to automatically create an `index.html` HTML file
**Improve development speed**
-   Modify the webpack config to support inline source mapping.
-   Check that the console.log in the header.js now takes you to your javascript file instead of the main bundle.
-   Add a plugin to Webpack to clean your build folder on each build.
**Improve bundles size:**
-   You can see that the current modules generated with `npm run build` are quite large. They all contain jQuery and/or Lodash. Modify the Webpack configuration to split the modules in chunks.
**Requirements:**
-   When running the dev server, your code should work on `http://localhost:8564/`.
-   When running Webpack, your javascript and html files should be generated in a `public` folder.
-   Opening your main file should not generate any error in the console.
**Repo:**
-   GitHub repository: `alx-react`
-   Directory: `0x00-Webpack`
-   File: `task_3/modules/body/body.css, task_3/modules/body/body.js, task_3/modules/footer/footer.css, task_3/modules/footer/footer.js, task_3/modules/header/header.css, task_3/modules/header/header.js, task_3/package.json, task_3/webpack.config.js`
 Done? Help Check your code
Copyright © 2022 ALX, All rights reserved.
