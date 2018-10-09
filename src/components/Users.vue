<template>
  <div class="users">
    <ul>
      <li v-for="user in users" v-on:click="user.show = !user.show">
        <h2>{{user.name}}</h2>
        <h3 v-show="user.show">{{user.position}}</h3>
      </li>
    </ul>
  </div>

</template>

<script>
    export default {
        name: "users",
        data(){
          return {
            users:[
              {'name':'henry','position':'web开发','show':false},
              {'name':'henry','position':'web开发','show':false},
              {'name':'henry','position':'web开发','show':false},
              {'name':'henry','position':'web开发','show':false},
              {'name':'henry','position':'web开发','show':false},
              {'name':'henry','position':'web开发','show':false}
            ]
          }
        }
    }
</script>

<style scoped>

</style>
