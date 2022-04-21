<template>
<section id="video_section">

 <div class="container-md"> <!-- switch to margin x over MD size(fluid and !fluid) -->
  <div class="row">



    
    <div >
      <h1>Videoer</h1>
    </div>
 

    
    

    <div v-for="portrait in portraits" :key="portrait" class="col-12 col-sm-6 col-md-4 mb-4" >
      <div class="card" style="">
       

    
        <YouTube 
        :src="portrait.projectURL"
        @ready="onReady"
        :width="testSizeOn.value"
        ref="youtube" />

        <div class="card-body justify-content-start">
          <h5 id="cardOne" class="card-title ">{{portrait.projectTitle}}</h5>
          <p class="card-text">{{portrait.projectDescription}}</p>
          
        </div>
      </div>
    </div>
{{testSize}}

  </div>
  
</div>
</section>
</template>

<script>
import { ref, computed} from 'vue'

import YouTube from 'vue3-youtube'

export default {
  components: { YouTube },

  setup() {
    
   //let ytWidth = ref('')

    let testSize = ref(
     window.innerWidth
    )
    let ytWidth = ref('')


    let testSizeOn = computed(()  => {
      
      if (testSize.value >= 1400) {
         return ytWidth = ref('414px')
         
      }
      else if (testSize.value >= 1200) {
        return ytWidth = ref('354px')
      }
      else if (testSize.value >= 1199 || testSize.value >= 992) {
        return ytWidth = ref('294px')
      }
      else if (testSize.value >= 576) {
        return ytWidth = ref('214px')
      }
      else if ( testSize.value >= 415 ) {
        return ytWidth = ref('548px')
      }
      else if (testSize.value <= 414 ) {
        return ytWidth = ref('370px')
      }
      else {
        return ytWidth = ref('')
      }
    })

    let onReady = () => {
        //    this.youtube.playVideo()
        }
 
    let portraits = ref([
      {
        projectID: 1,
        projectTitle: "Festoriginalerne",
        projectDescription: "Promovideo",
        projectURL: "https://www.youtube.com/watch?v=6zb7pitSQLE",
        projectCategory: "Video"
      }, 
       {
        projectID: 2,
        projectTitle: "Slideshow",
        projectDescription: "Lavet til min søsters bryllup",
        projectURL: "https://www.youtube.com/watch?v=mqaDKMhIn8A",
        projectCategory: "Video"
      },
      {
        projectID: 3,  
        projectTitle: "Esbjerg Bryghus",
        projectDescription: "En kort reklame lavet for Esbjerg Bryghus",
        projectURL: "https://youtu.be/hjwB2KrkUzs",
        projectCategory: "Video"
      },
      {
        projectID: 4,  
        projectTitle: "Trapholt",
        projectDescription: "En lille teaser for Trapholt",
        projectURL: "https://www.youtube.com/watch?v=-157TZOcSD8",
        projectCategory: "Video"
      },
      {
        projectID: 5,  
        projectTitle: "Festoriginalerne",
        projectDescription: "Sweet child of mine guitarsolo",
        projectURL: "https://www.youtube.com/watch?v=QHy0dHAE1t8",
        projectCategory: "Video"
      },
      {
        projectID: 6,  
        projectTitle: "Bryllupsslideshow",
        projectDescription: "Et slideshow lavet til min søsters bryllup",
        projectURL: "https://www.youtube.com/watch?v=YpvteIDz9d4&t=8s",
        projectCategory: "Video"
      },

])
    return {
      portraits,
      onReady,
      ytWidth,
      testSize,
      testSizeOn
      
    }
  }
}
</script>

<style scoped>

#video_section{
    background-color: #222;
}
 
h1{
  color: #edf1f5 ;}
  
#cardOne{
  color: #222; 
}
.active {
  background-color: khaki;
  
}
#yt-container {
      position: relative;
    width: 100%;
    height: 0;
    padding-bottom: 56.25%;
}
#yt-styling {
   position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}

.text-color {
  color:darkviolet;
}
</style>