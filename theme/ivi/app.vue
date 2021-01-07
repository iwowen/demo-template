<template>
  <div>
    <div v-for="(item, index) in pagesConfig" :key="index">
      <h2>{{ item.name }}</h2>
      <table>
        <thead>
          <tr>
            <th>标题</th>
            <th>分类</th>
            <th>name</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="(e, i) in item.pages" :key="i">
            <td>{{ e.title }}</td>
            <td>{{ e.type }}</td>
            <td>{{ e.name }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>
<script>
export default {
  computed: {
    pagesConfig() {
      return window.pagesConfig;
    },
  },
};
</script>
<style lang="css">
table {
  border-spacing: 0;
}
th,
td {
  border: 1px solid rgba(0, 0, 0, 0.1);
  padding: 10px 20px;
}
</style>
