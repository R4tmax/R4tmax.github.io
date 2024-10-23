# R4tmax.github.io
Underlying folder for https://r4tmax.github.io/.
See [Project Setup](#project-setup) for how to copy and reproduce deployment steps.

## License
All contents of this repo can be considered part of the Public Domain.

## Type Support for `.vue` Imports in TS

TypeScript cannot handle type information for `.vue` imports by default, so we replace the `tsc` CLI with `vue-tsc` for type checking. In editors, we need [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) to make the TypeScript language service aware of `.vue` types.

## Customize configuration

See [Vite Configuration Reference](https://vite.dev/config/).

## Project Setup

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Type-Check, Compile and Minify for Production

```sh
npm run build
```

### Lint with [ESLint](https://eslint.org/)

```sh
npm run lint
```
### Deploy to GH pages
First install npm gh-pages module.
```sh
npm install gh-pages --save-dev
```
Then update (or create) your *vue.config.js*

```js
module.exports = {
    publicPath: process.env.NODE_ENV === 'production'
      ? 'R4tmax.github.io'  // replace with your GitHub repo name
      : '/'
  }
```

Next, make sure that the scripts segment of package.json has: 
```js
"scripts": {
  "deploy": "gh-pages -d dist" // replace with your preffered branch name
}
```
For this step to work, make sure, that you have configured your GH repo correctly.
**Settings > Pages > set the source branch**

Once all of this is done, all you need is:
```sh
npm run deploy
```
For all subsequent deploys.
