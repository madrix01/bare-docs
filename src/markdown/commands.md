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

  Create boilerplate of the project from a current bare

## include

- Usage:
  ```
  bare include [<all the files you want to include>]
  ```
  This command to add `recipe.json` or add manually to `recipe.json` (we dont recommend to add manually)

## touch

- Usage:
  ```
  bare touch <touch-name> <destination>
  ```
  This command generates a copy of single boilerplate file from your Bare to project

## rm

- Usage:
  ```
  bare rm <bare-name>
  ```
  This command removes saved bare from `~/.bare`

## get

- Usage:
  ```sh
  bare get <username>/<template-repo>
  ```
  This command download any online template from github to `~/.bare` for future use
