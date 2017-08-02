# headless-example-vue

> Example project connected to the Headless CMS

This is simply the Vue webpack template.

Notable changes to integrate Headless CMS:

`build/headless.js` added

`headless/` contains downloaded content files

`src/components/Hello.vue` requires the JSON file

`npm run fetchContent` gets the content from the Content API

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
