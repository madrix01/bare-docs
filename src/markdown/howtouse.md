# Getting started

- [Install](/install) bare on your computer.

## Adding a current boilerplate

For this tutorial let us use a `express node js` project
Suppose you have made barebones for express app and want to use it later projects or in this one 
``` text 
|- src
|   |- index.js
|   |- routes
|       |- home.js
|       |- auth.js
|- package.json
|- Dockerfile
|- .eslintrc
```

- Lets start bare initalizing it as bare 
    ``` sh
    bare init <bare-name>
    ```
    For this tutorial we'll use `test` as bare-name 
    ``` sh
    bare init test
    ```
    This will create a file with `~/.bare/test`
    And a file with `recipe.json` in root of the project.

### Let's configure recipe.json 
To learn more about the recipe, click [here](/recipe)
