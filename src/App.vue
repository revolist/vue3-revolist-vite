<template>
  <v-grid theme="compact" :source="rows" :columns="columns"></v-grid>
</template>


<script lang="ts">
import { defineComponent } from "vue";
import VGrid from "@revolist/vue3-datagrid";
export default defineComponent({
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
    VGrid
  }
});
</script>
<style>
  revo-grid {
    height: 500px;
  }
</style>