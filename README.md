# VGreen Application - Frontend

## Steps

	1. Copy Files in your application.

	2. Go to App\Providers\RouteServiceProvider.php and change this:
        public const HOME = '/backend';

    3. Consuming Your API With JavaScript:
https://laravel.com/docs/7.x/passport#consuming-your-api-with-javascript

	4. Add in your main app.js:
```javascript
const moduleVueFiles = require.context('../../Modules', true, /\.vue$/i);
moduleVueFiles.keys().map(key => Vue.component(key.split('/').pop().split('.')[0], moduleVueFiles(key).default));
```
	5. NPM
```bash
npm install && npm run dev
```

## Assets Module

    - Install and Setup:
https://nwidart.com/laravel-modules/v6/basic-usage/compiling-assets