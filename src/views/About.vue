<template>
  <div class="home">
    <HelloWorld msg="about"/>
    
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
