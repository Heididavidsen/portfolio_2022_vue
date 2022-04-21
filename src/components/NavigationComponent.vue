<template>
    <div>
        <nav class="d-flex justify-content-center col-12">
            <div class="d-flex align-items-center justify-content-between col-12 ">
            <div class="navigation col-sm-4 col-md-2">
                <router-link to="/">Hjem</router-link>
      <!--           <a href="#picture_section">Billeder</a>
                <a href="#video_section">Videoer</a>-->
                <router-link to="/contact">Kontakt</router-link>



            </div>
            <div class="title_logo col-sm-4 col-md-2">
            
                <p>Sand Stories</p>

            </div>
                
            <div class="social_media col-sm-4 col-md-2">
                <a href="https://www.facebook.com/Sandstoriess" target="_blank"><i class="fa-brands fa-facebook-f"></i></a>
               <a href="https://www.linkedin.com/in/heididavidsensandstories/" target="_blank"> <i class="fa-brands fa-linkedin-in"></i></a>
               <a href="https://www.youtube.com/channel/UClB1FgpdUgKRxAEOTlr-aIQ" target="_blank"> <i class="fa-brands fa-youtube"></i></a>
               <a href="https://www.instagram.com/sandstoriesdk/" target="_blank"> <i class="fa-brands fa-instagram"></i></a>


            </div>
            </div>
            
        </nav>

    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>

nav {
  max-height: 14vh;  
  align-items: center;
  background-color: #0D0D0D;
  color: #edf1f5;
  .navigation{
      a{
          padding: 10px;
          text-decoration: none;
          &.router-link-exact-active {
        font-weight: bold;
      
    }
      }
  }
  .title_logo{
      font-family: "Great Vibes", Avenir, Helvetica, Arial, sans-serif;
        margin: 0px;
        font-size: 30px;
        font-weight: bold;


  }

  .social_media{
      i{padding: 10px;}

  }

  a {
    font-weight: bold;
    color: #edf1f5;

    
  }
}

</style>
