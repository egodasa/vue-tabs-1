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

