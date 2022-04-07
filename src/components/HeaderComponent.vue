<template>
  <div>
    <header>
      <div id="top-header">
        <!-- Logo -->
        <div id="logo">
          <img alt="Vue logo" height="40" src="../assets/logo.png">
        </div>
      </div>

      <div id="navigation" class="outer-col-12">
        <nav>
          <router-link to="/">Hjem</router-link> | 
          <router-link to="/about">About</router-link>
        </nav>
        <router-view />
      </div>
    </header>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
    header {
  height:200px;
  background-color: white;
  display: flex;
  flex-wrap: wrap;
  gap: 0px;
  max-width: 80vw; // Change for full width or a set width -> in config file
  width: 80vw;
  justify-content: center;
  margin-bottom:30px;
  nav {
    justify-content: center;
    border-top: 1px solid #333333;
    border-bottom: 1px solid #333333;
    display: flex;
    align-items: center;
    width: 100%;
    ul {
      display: flex;
      list-style-type: none;
      li {
        padding:0 10px;
        a {
          color: lelele;
          &:hover {
            color: black;
          }
        }
      }
    }
  }
}

</style>   