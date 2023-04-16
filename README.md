# Imps Skeleton Loader

Skeleton loader vue component. Working on vue2 and vue3 both

[![N|Solid](https://www.iampapaisarkar.in/powered-by.svg)](https://www.iampapaisarkar.in)

[![N|Solid](https://www.iampapaisarkar.in/hire-me.svg)](https://www.upwork.com/freelancers/~01b68508e481c72291)

## Documentation
see documentation [here](https://www.iampapaisarkar.in/npm-packages.html#skeleton-loader)

## installation
### Vue2
```sh
npm i imps-skeleton-loader --tag=v2
```
### Vue3
```sh
npm i imps-skeleton-loader --tag=v3
```
## Usage

```vue
#Vue 2 
// import and use in your main.js file

import Vue from 'vue'
import App from './App.vue'
import ImpsSekeletonLoader from 'imps-skeleton-loader';

Vue.use(ImpsSekeletonLoader);

new Vue({
  render: h => h(App),
}).$mount('#app')

```

```vue
// use on vue components 

<template>
  <div>
    <imps-skeleton-loader width="100px" height="100px" round="100px"/>
  </div>
</template>

```

```vue
#Vue 3 
// import and use in your main.js file

import { createApp } from 'vue';
import App from './App.vue';
import ImpsSekeletonLoader from 'imps-skeleton-loader';

const app = createApp(App);

// Install the plugin globally
app.use(ImpsSekeletonLoader);

app.mount('#app');
```

```vue
// use on vue components 

<template>
  <div>
    <imps-skeleton-loader width="100px" height="100px" round="100px"/>
  </div>
</template>

```
## License

[MIT](https://choosealicense.com/licenses/mit/)