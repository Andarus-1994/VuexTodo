<template>
  <div class="filter">
    <label>Filter Todos:</label>
    <select @change="filterTodos($event)">
      <option value="200">200</option>
      <option value="100">100</option>
      <option value="50">50</option>
      <option value="20">20</option>
      <option value="10">10</option>
      <option value="5">5</option>
    </select>
  </div>
</template>

<script>
import { mapActions } from "vuex";
export default {
  name: "FilterTodos",
  methods: mapActions(["filterTodos"]),
};
</script>

<style scoped>
select {
  margin-top: 20px;
  padding: 6px;
  border: rgb(110, 156, 92) 1px solid;
  margin-left: 10px;
}
</style>
