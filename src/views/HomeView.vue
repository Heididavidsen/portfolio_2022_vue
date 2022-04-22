<template>
  <div class="home">
    <div class="parallax-one">
      <h1 id="headline">
          Heidi Davidsen.
          </h1>
           <br />
          <p id="velkommen"> Velkommen til mit portfolio. Her kan du se, hvilke projekter jeg har arbejdet med. <br /> 
          Jeg arbejder med design til poster, logo, hjemmesider, visitkort, foldere, foto og videoprojekter. 
         </p> 
         

    </div>
    <div class="row-links">
      <h2 id="headline2">
        Billeder
      </h2>
    <router-link to="/picture"> 
      <img id="picture_img_link" src="../assets/omvendt.jpg" alt="">
    </router-link>
    </div>

    <div class="row-links">
      <h3 id="headline3">
        Videoprojekter
      </h3>
     <router-link to="/video">  
     <img id="picture_img_link" src="../assets/festoriginalerne.jpg" alt=""></router-link>
     </div>

     <div class="row-links">
       <h4 id="headline4">
        Logo/Poster
      </h4>
      <router-link to="/logo/">  <img id="picture_img_link" src="../assets/sandstorieslogo.png" alt=""></router-link>
</div>
<!--
    <PictureComponent />
    -->
    
    <VideoComponent />
    <LogoComponent />
  </div>
</template>

<script>
// @ is an alias to /src
//import PictureComponent from "@/components/PictureComponent.vue";
//import VideoComponent from "@/components/VideoComponent.vue";
//import LogoComponent from "@/components/LogoComponent.vue";

export default {
  name: "HomeView",
  components: {
  //  PictureComponent,
  //  VideoComponent,
  //  LogoComponent
  },
};
</script>

<style scoped>
.parallax-one {
  padding-top: 400px;
  padding-bottom: 400px;
  overflow: hidden;
  position: relative;
  width: 100%;
  background-image: url("../assets/sidderpaastol-dark.png");
  background-attachment: fixed;
  background-size: cover;
  -moz-background-size: cover;
  -webkit-background-size: cover;
  background-repeat: no-repeat;
  background-position: top center;

  position: relative;

}
#headline{
  font-family: "Great Vibes", Avenir, Helvetica, Arial, sans-serif;
  color: #edf1f5;
  font-weight: bold;
  font-size: 60px;
  

  }

#velkommen{
  color: #edf1f5;
  font-size: 20px;
}  
#headline2{
  color: #edf1f5;
}
#headline3{
  color: #edf1f5;
}
#headline4{
  color: #edf1f5;
}

.row-links {
 
  background-color: #222;
  padding:20px 0
}
.row-links img {
   filter: grayscale(100);
}

.row-links img:hover{
   filter: grayscale(0);
   
}

#picture_img_link {
  height:90vh;
  width: 90vw;
  
}
</style>




