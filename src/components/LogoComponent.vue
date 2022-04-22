<template>

<section id="logo_section">

 <div class="container-md"> <!-- switch to margin x over MD size(fluid and !fluid) -->
  <div class="row">



    
    <div >
      <h1>Logo/Poster</h1>
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
        projectTitle: "Halloweenplakat",
        projectDescription: "Poster",
        projectURL: require("../assets/halloween.png"),
        projectCategory: "Video"
      }, 
       {
        projectID: 2,
        projectTitle: "Trapholt",
        projectDescription: "Logo med farve",
        projectURL: require("../assets/logoexam.jpg"),
      },
      {
        projectID: 3,  
        projectTitle: "Trapholt",
        projectDescription: "Logo sort/hvid",
        projectURL: require("../assets/trapholtsort.png"),
      },
      {
        projectID: 4,  
        projectTitle: "Sand Stories",
        projectDescription: "Eget design af logo",
        projectURL: require("../assets/sandstorieslogo.png"),
      },
      {
        projectID: 5,  
        projectTitle: "Seed of Life Logo",
        projectDescription: "Logo lavet til holistisk terapi",
        projectURL: require("../assets/seedoflife.png"),
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
    height: 200vh;
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