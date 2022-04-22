<template>
<section id="picture_section">

 <div class="container-md"> <!-- switch to margin x over MD size(fluid and !fluid) -->
  <div class="row">



    
    <div >
      <h1>Billeder</h1>
    </div>
 

    
    

    <div     v-for="portrait in portraits" :key="portrait" class="col-12 col-sm-6 col-md-4 mb-4" >
      <div class="card" style="">
        <img :src="portrait.projectURL" class="card-img-top" alt="...">
        <div class="card-body justify-content-start">
          <h5 id="cardOne" class="card-title ">{{portrait.projectTitle}}</h5>
          <p class="card-text">{{portrait.projectDescription}}</p>
          
        </div>
      </div>
    </div>


  </div>
  
</div>
</section>
</template>

<script>
import { ref } from 'vue'
export default {
  setup() {
    
    
 
    let portraits = ref([
      {
        projectID: 1,
        projectTitle: "Familiebilleder",
        projectDescription: "Photoshoot i skoven",
        projectURL: require("../assets/pborn.jpg"),
        projectCategory: "Video"
      }, 
       {
        projectID: 2,
        projectTitle: "Portræt",
        projectDescription: "Photoshoot i skoven",
        projectURL: require("../assets/skoveli.jpg"),
      },
      {
        projectID: 3,  
        projectTitle: "Portræt",
        projectDescription: "Photoshoot i skoven",
        projectURL: require("../assets/nickey.png")
      },
      {
        projectID: 4,  
        projectTitle: "Esbjerg Bryghus",
        projectDescription: "Firmabilleder",
        projectURL: require("../assets/esbjergbryghus.jpg")
      },
      {
        projectID: 5,  
        projectTitle: "Esbjerg Bryghus",
        projectDescription: "Firmabilleder",
        projectURL: require("../assets/esbbryg.jpg")
      },
      {
        projectID: 6,  
        projectTitle: "Esbjerg Bryghus",
        projectDescription: "Firmabilleder",
        projectURL: require("../assets/esbjbryg.jpg")
      },{
        projectID: 7,  
        projectTitle: "Hjerting Strand",
        projectDescription: "Børn",
        projectURL: require("../assets/nick.jpg")
      },{
        projectID: 8,  
        projectTitle: "Hjerting Strand",
        projectDescription: "Glaskugle",
        projectURL: require("../assets/kugle.jpg")
      },{
        projectID: 9,  
        projectTitle: "Hjerting Strand",
        projectDescription: "Glaskugle",
        projectURL: require("../assets/kuglestr.jpg")
      },
      {
        projectID: 10,  
        projectTitle: "Mia's konfirmation",
        projectDescription: "Konfirmand 2021",
        projectURL: require("../assets/konfirmationgul.jpg")
      },{
        projectID: 11,  
        projectTitle: "Mia's konfirmation",
        projectDescription: "Konfirmand 2021",
        projectURL: require("../assets/taarer.jpg")
      },{
        projectID: 12,  
        projectTitle: "Mia's konfirmation",
        projectDescription: "Konfirmand 2021",
        projectURL: require("../assets/konfimia.jpg")
      },
      {
        projectID: 13,  
        projectTitle: "St Darum Kirke",
        projectDescription: "Snelandskab",
        projectURL: require("../assets/kirke.jpg")
      },{
        projectID: 14,  
        projectTitle: "St Darum Kirke",
        projectDescription: "Snelandskab",
        projectURL: require("../assets/kirkesne.jpg")
      },{
        projectID: 15,  
        projectTitle: "Snebillede",
        projectDescription: "Snelandskab",
        projectURL: require("../assets/sne.jpg")
      },
      
    ])
    return {
      portraits,
    
      
    }
  }
}
</script>

<style scoped>

#picture_section{
    background-color: #222;
    
}
 
h1{color: #edf1f5 ;}
#cardOne{
  color: #222; 
}

#video_section{
    background-color: #222;
    height: 200vh;
    
}
.active {
  background-color: khaki;
  
}
.text-color {
  color:darkviolet;
}
</style>