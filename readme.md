# esbuild + Snowpack + Preact + TypeScript starter
This project is a POC implementation of building a web-app with preact and TypeScript, with esbuild as the transpiler + bundler + minifier, but Snowpack on development.

The idea is to have a very fast development server to allow fastest possible feedback loop on development using Snowpack, and use esbuild to bundle really fast for production.

This project builds in 30-40ms. These numbers are taken on a MacBook Pro 13" 2020. 

This is basically adding snowpack to [esbuild-preact-typescript-starter](https://github.com/jackyef/esbuild-preact-typescript-starter)

## Includes
- [**Snowpack**](https://github.com/snowpackjs/snowpack), for a crazy fast development workflow
- [**esbuild**](https://github.com/evanw/esbuild), for bundling, transpiling, minifying, and generating source maps
- [**Preact**](https://github.com/preactjs/preact), UI runtime
- [**TypeScript**](https://www.typescriptlang.org/)
- [**Goober**](https://github.com/cristianbote/goober), a less than 1KB css-in-js solution

## Instructions
1. Before doing anything, install the dependencies
    ```
    yarn
    ```

2. Run the following the start the development server
    ```
    yarn dev
    ```

3. Make changes as you need, the changes will be reflected automatically in the browser

4. When you are ready to bundle to production:
    ```
    yarn build
    ```

5. Test serving the production bundle locally
    ```
    yarn serve
    ```

## Caveats
- Please refer to [esbuild-preact-typescript-starter](https://github.com/jackyef/esbuild-preact-typescript-starter#caveats) for the caveats of using esbuild for production build.
