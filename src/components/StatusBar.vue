<template>
  <div class="status-bar" v-if="auth.isAuthenticated">  
      <p>Done</p>
      <ul>
          <li v-for="todo in doneTodos" :key="todo.id">{{todo.title}}</li>
      </ul>
  </div>
</template>

<script>

import {mapGetters, mapState} from 'vuex'
export default {
    name: 'StatusBar',
    computed: {...mapGetters(['doneTodos']), ...mapState(['auth'])}
    
}
</script>

<style>

</style>


