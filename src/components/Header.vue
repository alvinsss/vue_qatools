<template>
  <header>
    <h1>{{title}}</h1>
  </header>
</template>

<script>
export default {
  name: 'app-header',
  data () {
    return {
      title: '和信测试工具导航'
    }
  }
}
</script>

<style scoped>
  header{
    background:lightgreen;
    padding: 10px;
  }

  h1{
    color:#222;
    text-align: center;
  }

</style>
