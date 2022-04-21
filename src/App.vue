<template>
  <div id="toplevel-wrapper" class="container-fluid d-flex min-vh-100 flex-column">
    <NavigationComponent />
    <router-view/>
  
  </div>  
</template>

  <script>
  import NavigationComponent from '@/components/NavigationComponent.vue'
  export default {
    components: {NavigationComponent}
    
  }
  </script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  #toplevel-wrapper { 
  padding:0; /* Added */
  

}
}


</style>
