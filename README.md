# react-typescript-snowpack

A step-by-step commit by commit development for a react typescript app with snowpack build which can serve as a tutorial.

Note: Because we start from scratch and add snowpack, react and typescript in that order, this tutorial is also helpful for development in other frameworks.

# Activity

1. Created an npm package and marked it private.
2. Install snowpack as dev dependency.
3. Run snowpack dev server.

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
