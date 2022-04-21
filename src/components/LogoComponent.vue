<template>
<section id="logo_section">

 <div class="container-md"> <!-- switch to margin x over MD size(fluid and !fluid) -->
  <div class="row">



    
    <div >
      <h1>Logoer</h1>
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
        projectTitle: "Firmabilleder",
        projectDescription: "Esbjerg Bryghus",
        projectURL: require("../assets/esbjergbryghus.jpg"),
      },
      {
        projectID: 3,  
        projectTitle: "Card Two",
        projectDescription: "Lorem ipsum, text is very nice. Much wow2",
        projectURL: "https://images.unsplash.com/photo-1572177812156-58036aae439c?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MXx8cHJvamVjdHN8ZW58MHx8MHx8&w=1000&q=80"
      },
      
    ])
    return {
      portraits,
    
      
    }
  }
}
</script>

<style scoped>

#logo_section{
    background-color: #222;
}
 
h1
{color: #edf1f5 ;}

#cardOne{
  color: #222; 
}
.active {
  background-color: khaki;
  
}
.text-color {
  color:rgb(247, 245, 248);
}
</style>