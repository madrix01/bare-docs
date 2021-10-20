# Installation

### 🐧 Currently bare is only available for linux

- To install bare you must have npm installed
  ```
  npm i -g barego
  ```
- To check installation
  ```
  bare
  ```

### To install nighly build

```
npm i -g madrix01/bare#dev
```

- Revert it back using the installing

  ```
  npm i -g barego
  ```

### To build from source

Thank you for interest in our project. We appreciate the time you took for contributing. Follow the steps to get started.

## Steps for setup

- Fork the repo from [here](https://github.com/bare-cli/bare)
- Clone the forked repo by git:

  ```
  git clone https://github.com/<username>/bare <folder-name>
  ```

  or by [gh](https://github.com/cli/cli) :

  ```
  gh repo clone <username>/bare <folder-name>
  ```

- Change directory to your local copy:
  ```
  cd <folder-name>
  ```
- (Optional) if shell errors out
  ```
  go mod tidy
  ```
- Build the tool using make:
  ```
  make build
  ```

Now you will have your tool in `bin` folder, you can try it out following `Readme.md`.
