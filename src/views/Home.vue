<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/basketball-ball-solid.svg">
    <HelloWorld msg="test"/>
    
  </div>
  
</template>
<i class="fas fa-basketball-ball"></i>
<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  components: {
    HelloWorld
  }
}
</script>
