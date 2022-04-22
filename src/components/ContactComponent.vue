<template>


<section id="contact_section" class="d-flex justify-content-center">

 
  

    

    <div class="col-12 col-sm-6 col-md-4 mb-4 "  >
          <h1>Kontakt</h1>
      <form class="row g-3">
      <div class="col-md-12">
        <label for="inputEmail4" class="form-label">For mere info</label>
        <input type="email" class="form-control" placeholder="Email"  id="inputEmail4">
       </div>

      <div class="input-group">

        <textarea class="form-control" placeholder="Skriv besked" aria-label="With textarea"></textarea>
      </div>

 


      <div class="col-12">
        <button type="submit" class="btn btn-light">Send</button>
      </div>
      </form>
            <div class="cv-video">

              <iframe width="560" height="315" src="https://www.youtube.com/embed/V3HrX6CWxn4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
           </div>
           <div class="cv"><a target="_blank" class="btn btn-light btn-lg" href="https://firebasestorage.googleapis.com/v0/b/portfolio-2022-vue.appspot.com/o/CV%20.pdf?alt=media&token=c565730f-75a4-41c5-a472-6daf7a386be0">Link til CV</a>
            </div>
    </div>

  
  

</section>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
form {
  color:white
  
}
#contact_section{
    background-color: #222;
    height:100vh;
}
 
h1{color: #edf1f5 ;
text-align: center;
margin-top: 20px;
margin-bottom: 50px ;}


#input-group{
  justify-content: center;
  
}
.cv-video {
  position: relative;
  top: 50px;
  bottom: 50px;
 
  
  

}
.cv{
  position: relative;
  top: 130px;
}


 
.active {
  background-color: khaki;
  
}
.text-color {
  color:darkviolet;
}
</style>
