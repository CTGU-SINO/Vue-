<template>
    <footer>
      <h1>{{CopyRight}}</h1>
    </footer>
</template>

<script>
    export default {
        name: "footer",
        data(){
          return {
            CopyRight:'Copyright 2017 Vue Demo'
          }
        }
    }
</script>

<style scoped>
  footer{
    background: gray;
    padding: 10px;
  }
  h1{
    color: #222;
    text-align: center;
  }
</style>
