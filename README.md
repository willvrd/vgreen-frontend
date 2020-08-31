# VGreen Application - Frontend

## Steps

	1. Copy Files in your application

## VueJS Components

	1. Add in your main app.js:

```javascript
const moduleVueFiles = require.context('../../Modules', true, /\.vue$/i);
moduleVueFiles.keys().map(key => Vue.component(key.split('/').pop().split('.')[0], moduleVueFiles(key).default));
```

	2. NPM
```bash
npm install && npm run dev
```

## Assets Module

    - Install and Setup:
https://nwidart.com/laravel-modules/v6/basic-usage/compiling-assets