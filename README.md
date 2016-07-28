# vue-tabs

> Tabs implementation with Vue.js and Bootstrap

![animation](https://cloud.githubusercontent.com/assets/1509692/17219490/f30bae36-54c1-11e6-949e-606e944f695d.gif)

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build
```

## Simple Usage

```
<tabs>
  <tab name="t1" title="Tab 1" active=true>
    Hello World
  </tab>
  <tab name="t2" title="Tab 2">
    Hello World 2
  </tab>
  <tab name="t3" title="Tab 3">
  Hello World 3
  </tab>
</tabs>
```

## A bit complex

```
<template>
  <div id="app" class="container">
    <h1> Tabs </h1>
    <tabs>
      <tab name="t1" title="Tab 1" active=true>
        Hello World
      </tab>
      <tab name="t2" title="Tab 2">
        <simple-table></simple-table>
      </tab>
      <tab name="t3" title="Tab 3">
        <simple-form></simple-form>
      </tab>
    </tabs>
  </div>
</template>
<script>
  import Tabs from './components/Tabs.vue'
  import Tab from './components/Tab.vue'
  import SimpleTable from './views/SimpleTable.vue'
  import SimpleForm from './views/SimpleForm.vue'

  export default {
    components: {
      Tabs,Tab,
      SimpleForm,SimpleTable
      }
    }
</script>
```

