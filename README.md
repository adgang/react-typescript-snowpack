# react-typescript-snowpack

A step-by-step commit by commit development for a react typescript app with snowpack build which can serve as a tutorial.

Note: Because we start from scratch and add snowpack, react and typescript in that order, this tutorial is also helpful for development in other frameworks.

# Activity

1. Created an npm package and marked it private.
2. Install snowpack as dev dependency.
3. Run snowpack dev server.
4. Add snowpack config.
5. Add javascript file.
6. Use typescript file.

## 1. Created an npm package


```
npm init
```

Added LICENSE and README

## 2. Install snowpack

We first install snowpack as a dev dependency.

```
npm install --save-dev snowpack
```

## 3. Run dev server

We create a html and serve it with snowpack dev server. The smart defaults of snowpack ensure that we just need to create an `index.html` file in the project folder and run:

```
npx snowpack dev
```

We then added `npm start` script to `package.json`.

## 4. Add snowpack config
We notice that even git commands are triggering updates to the page. To make snowpack ignore changes in `.git` folder, we add a config file `snowpack.config.js`. We annotate the config object for typescript information in vscode.

To make this step easier, generate a config file first with `npx snowpack init` and then add configure excludes option to `node_modules` and `.git` folders.

## 5. Add javascript file
Have dev tools open on browser and add a js file `index.js` and src it in the html. The file loads as can be evidenced by log.

Until now, we could have been developing in any framework like Vue, svelte etc., There would be no difference.

## 6. Use typescript file
Rename `index.js` file to `index.ts` and see that the log is still displayed. Snowpack is able to convert the ts into js and link it from `index.html`
