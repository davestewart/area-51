# Area 51

> Nuxt Areas external area demo

<p align="center">
  <img src="https://raw.githubusercontent.com/davestewart/area-51/master/docs/area-51.png" alt="Area 51">
</p>

## Overview

[Nuxt Areas](https://github.com/davestewart/nuxt-areas) is a Nuxt module that enables you to structure your Nuxt site by "area":

```
+- src
    +- areas
        +- products
        |   +- ...
        +- users
            +- components
            +- pages
            +- store
```

In addition to local folders, Areas lets you include external areas via path or NPM module.

This is an installable demo module to show you how it works.

## Usage

In your Nuxt project, install Nuxt Areas and this demo area:

```bash
npm i nuxt-areas davestewart/area-51
```

If you don't have a project set up, you can use the main [Nuxt Areas Demo](https://github.com/davestewart/nuxt-areas-demo).

In your project's `nuxt.config.js` set up Areas as a build module, and configure Areas to load the demo area:

```js
export default {
  buildModules: [
    'nuxt-areas',
  ],

  areas: {
    external: [
      {
        src: 'area-51',     // package name 
        route: '/fifty-one' // route you want to view the pages on
      },
    ]
  }
}
```

To view the installed area in your browser:

- run the project via `npm run dev` 
- navigate to `http://localhost:3000/fifty-one` (or equivilent)

