---
layout: default
title: Frontend VueJS Nuxt
parent: Course Supplementary
grand_parent: Tutorials - Video
published: true
---
<h6>Course: Supplementary Technology</h6>
<h1 style="margin-top:0">Frontend VueJS + Nuxt</h1>


## Install Node and NPM or Yarn

Follow the instruction below to install npm.

Reference: https://radixweb.com/blog/installing-npm-and-nodejs-on-windows-and-mac


## Installation Nuxt

VueJS gets installed with Nuxt

```bash
npm init nuxt-app {app_name}
```

### Selections
* Project name: {your project name}
* Programming language:  **JavaScript**
* Package manager: **NPM** 
* UI framework: **Vuetify.js**
* Nuxt.js modules: **Axios**
* Linting tools: **ESLint**
* Testing framework: **None**
* Rendering mode: **Single Page App**
* Deployment target: **Static** (Static/Jamstack hosting) 
* Development tools: No selection
* What is your GitHub username?
* Version control system: No selection

Only if needed, install the plugins separately.

```bash
vue add vuetify
yarn add @nuxtjs/axios
npm i eslint-plugin-vue
```
Reference  https://coreui.io/

## Nuxt Authentication

```bash
yarn add --exact @nuxtjs/auth-next
yarn add @nuxtjs/axios
```

Reference https://auth.nuxtjs.org/guide/setup/

## Troubleshoot
### Cannot find module 'vuetify/es5/util/colors' 
Solution
yarn add --dev @nuxtjs/vuetify
https://www.npmjs.com/package/@nuxtjs/vuetify

### node:internal/crypto/hash:67
  this[kHandle] = new _Hash(algorithm, xofLen);
Solution
export NODE_OPTIONS=--openssl-legacy-provider

### Error: No ESLint configuration found in
Solution
npm install eslint -g -D
eslint --init

### Error  Parsing error: Invalid ecmaVersion
Solution
Add in the .eslintrc.json
    "parserOptions": {
        "ecmaVersion": 2020,
        "sourceType": "module",
        "ecmaFeatures": {
            "globalReturn": false,
            "impliedStrict": false,
            "jsx": false
        }
    },
https://github.com/vuejs/vue-eslint-parser



{: .fs-6 .fw-300 }