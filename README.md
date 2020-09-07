# vue-dynamic-height

A light weight Vue plugin to let the height of your textarea component dynamic.

## Demonstration 👀 

![Vue Dynamic Height Sample](https://user-images.githubusercontent.com/11657454/92419946-e75f2b00-f146-11ea-88dd-2f6357e2ace9.gif)


## How to 🤔 

```
npm install --save vue-dynamic-height
```

### Use locally 📍 

```vue
<template>
  <textarea v-dynamic-height></textarea>
</template>

<script>
import dynamicHeight from 'vue-dynamic-height';

export default {
  name: MySampleTextareaComponent,
  directives: {
    dynamicHeight,
  },
};
</script>
```

### Use globally 🌐 

```js
import Vue from 'vue';
import { installVueDynamicHeight } from 'vue-dynamic-height';

Vue.use(installVueDynamicHeight);
```

## API 🔌 

### Config options

| Prop | Required | Default | Type | Description |
|---|---|---|---|---|
| `disabled` | No | false | Boolean | It disables the directive behavior. |
| `minHeight` | No | '0px' | String | Defines style a minimum height for textarea input |

### Usage

```vue
<template>
  <textarea v-dynamic-height="configObject"></textarea>
</template>
```

## Contribution 🚀 

Want to contribute? Feel free to open up an issue and/or a pull request here. 🙂 

At first, install all dependencies.
```
npm install
```

To run all tests, please run it.
```
npm test
```

To build you result, just do it.
```
npm run build
```

### Note ℹ️ 

To play with your result, you might run the command [`npm pack`](https://docs.npmjs.com/cli-commands/pack.html) to generate a compressed `.tgz` file. So far, you can install it within your own project and test it as long as you wish.

For example, browse your terminal to your own project repository path and run a command like this below:

```
npm install --save ../vue-dynamic-height/vue-dynamic-height-1.0.1.tgz
```


## License 📜 

[MIT](https://github.com/guibrancopc/vue-dynamic-height/blob/master/LICENSE)
