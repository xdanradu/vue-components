# @xdanradu/vue-components

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).


### Usage in external Vue project

```
npm install  @xdanradu/vue-components -D
```

Usage:
```html
<template>
  <div id="app">
    <Banner msg="this is a test banner"></Banner>
    <div class="photos">
    <Photo path="https://homepages.cae.wisc.edu/~ece533/images/airplane.png"></Photo>
    <Photo path="https://homepages.cae.wisc.edu/~ece533/images/baboon.png"></Photo>
    <Photo path="https://homepages.cae.wisc.edu/~ece533/images/boat.png"></Photo>
    <Photo path="https://homepages.cae.wisc.edu/~ece533/images/peppers.png"></Photo>
    <Photo path="https://homepages.cae.wisc.edu/~ece533/images/serrano.png"></Photo>
    </div>
  </div>
</template>

<script>
import "@xdanradu/vue-components/dist/xdanradu.css"
import Components from '@xdanradu/vue-components';

export default {
  name: 'App',
  components: {
    ...Components
  }
}
</script>

```

# TODO

- Minify the lib deployment package and exclude the src from npmjs (Keep the link to Github repo in the Readme file)
- Automate the deployment to npmjs through a github hook
- Components showcase (also built in this lib project) deployed on Heroku

Extra libs to play with: 

- https://lodash.com
- https://www.npmjs.com/package/chalk (Backend)
- https://www.npmjs.com/package/commander (CLI tools)
- https://www.npmjs.com/package/moleculer (Microservices)


Git repo: https://github.com/xdanradu/vue-components


### Usage as web component

```bash
    npm run build-web-components
```

```html
<script src="https://unpkg.com/vue"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/webcomponentsjs/1.2.0/webcomponents-loader.js"></script>
<script src="./my-custom-element.js"></script>
<my-custom-element msg="Hello web components"></my-custom-element>
```
