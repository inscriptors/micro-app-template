# MonorepoTemplate

[Add Github Actions Badge here]

<a alt="Nx logo" href="https://nx.dev" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/nrwl/nx/master/images/nx-logo.png" width="45"></a>

✨ **This workspace has been generated by [Nx, a Smart, fast and extensible build system.](https://nx.dev)** ✨

## Understand this workspace

This workspace has frontend project and a backend project.

Frontend project is React based and backend project is Express based.

### Build

To build the project run `yarn build` or `lerna run build` in the root directory.

This builds both the frontend and backend projects.

Build output is in the `dist` directory.

There are two builds for frontend. Once is for Single SPA and another one is for Webpack 5.

This project is a mono repo that utilizes nx and lerna to create a micro app chatbot component that can be seamlessly incorporated into any web application. It offers two integration options: Single SPA and Webpack 5 Module Federation.

## Installation

    Clone the repository:
    Navigate to the project directory: cd chatbot
    Install dependencies: yarn install

## Integration Options

### Single SPA:

    To integrate the chatbot component into your web application using Single SPA:
    Add Single SPA reference and understand its usage and configuration.
    Visit [Single SPA](https://single-spa.js.org/docs/getting-started-overview) for more information.
    Import the chatbot component into your Single SPA configuration.
    Customize the chatbot's appearance and behavior based on your application's requirements.

### Webpack 5 Module Federation:

    To incorporate the chatbot component using Webpack 5
    Familiarize yourself with Webpack 5 Module Federation. Learn how to share code and components across multiple applications. Visit Webpack 5 Module Federation for more details.
    Configure your Webpack setup to include the chatbot module.
    Customize the chatbot's styling and functionality to suit your application's needs.

## Remote caching

Run `npx nx connect-to-nx-cloud` to enable [remote caching](https://nx.app) and make CI faster.

## Further help

Visit the [Nx Documentation](https://nx.dev) to learn more.

## commitlint

This project uses [commitlint](https://commitlint.js.org/#/) to enforce commit message conventions. The commit message conventions are defined in the [commitlint.config.js](commitlint.config.js) file.

## Husky

This project uses [husky](https://typicode.github.io/husky/#/) to run git hooks. The git hooks are defined in the [husky.config.js](husky.config.js) file.

as part of yarn install husky will run `husky install` which will create a `.husky` directory and add a `pre-commit` hook to the `.git/hooks` directory. The `pre-commit` hook will run `yarn lint` before allowing a commit to be made.

```
npx husky add .husky/pre-commit "npx lint-staged"
```

```
# .husky/commit-msg (v8)
npx --no -- commitlint --edit $1
```

```
npx husky add .husky/commit-msg "npx --no -- commitlint --edit $1"
```

