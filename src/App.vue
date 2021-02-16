<template>
  <v-grid theme="compact" :source="rows" :columns="columns"></v-grid>
</template>


<script>
import { defineComponent } from "vue";
import HelloWorld from "./components/HelloWorld.vue";
import VGrid from "@revolist/vue3-datagrid";
export default defineComponent({
  name: "App",
  data() {
    return {
      columns: [{ prop: "name" }, { prop: "details" }],
      rows: [
        {
          name: "1",
          details: "Item 1"
        }
      ]
    };
  },
  components: {
    HelloWorld,
    VGrid
  }
});
</script>