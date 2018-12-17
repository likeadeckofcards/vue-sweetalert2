# vue-sweetalert2

[![npm](https://img.shields.io/npm/v/vue-sweetalert2.svg)](https://www.npmjs.com/package/vue-sweetalert2)

Vue.js wrapper for SweetAlert2. With support SSR.

![VueSweetalert2](assets/logo.png)

# [Demo](https://avil13.github.io/vue-sweetalert2/)

![vue-sweetalert2 demo](assets/vue-sweetalert2.gif)

---

## Get started


```bash
npm install -S vue-sweetalert2
```


```js
// main.js
import Vue from 'vue';
import VueSweetalert2 from 'vue-sweetalert2';

Vue.use(VueSweetalert2);
```

Now in the global object, you can access all the methods of [sweetalert2](https://github.com/limonte/sweetalert2).

If you want to add global options like button colors, do something like this:
```js
// main.js
import Vue from 'vue';
import VueSweetalert2 from 'vue-sweetalert2';

const options = {
  confirmButtonColor: '#41b882',
  cancelButtonColor: '#ff7674'
}

Vue.use(VueSweetalert2, options)
```


```html
// example-vue-component.vue
<template>
    <button v-on:click="showAlert">Hello world</button>
</template>

<script>
export default {
    methods: {
        showAlert(){
            // Use sweetalert2
            this.$swal('Hello Vue world!!!');
        }
    }
}
</script>
```

// Or
```js
Vue.swal('Hello Vue world!!!');
```

## Nuxt.js

Install dependencies:

```bash
npm install -S vue-sweetalert2
```

Add `vue-sweetalert2/nuxt` to modules section of `nuxt.config.js`

```js
{
  modules: [
    'vue-sweetalert2/nuxt'
  ]
}
```

Or pass in global options like this:

```js
{
  modules: [
    [
      'vue-sweetalert2/nuxt',
      {
        confirmButtonColor: '#41b882'
      ff7674
    ]
  ]
}
```


## The documentation for `sweetalert2`, you can find [here](https://sweetalert2.github.io/).
