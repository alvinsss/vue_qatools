<template>

  <footer>
    <p>{{copyright}}</p>
  </footer>

</template>

<script>
export default {
  name: 'app-footer',
  data () {
    return {
      copyright: 'Copyright   2019 ， create By hexindai QA team'
    }
  }
}
</script>

<style scoped>
  footer{
    background:#222;
    padding: 7px;
  }

  footer p{
    color:lightgreen;
    text-align: center;
  }

</style>
