# Commands

## init
- Usage:
    ```
    bare init <bare-name>
    ```
    - Initializes your current project with bare.
    - Creates a `recipe.json` file in the root of the project.
    - Creates an empty folder `~/bare/<bare-name>`
## add
- Usage:
    ```
    bare add
    ```
    - Reads `recipe.json` file from root and adds all the file to bare directory
    - know more about `recipe.json`
## list
- Usage:
    
    For list of all the bares use
    ```
    bare list
    ```
    For list of all the file in a bare use
    ```
    bare list <bare-name>
    ```
## use
- Usage:

    ```
    bare use <bare-name> <destination>
    ```
    Create barebones of the project from a current bare