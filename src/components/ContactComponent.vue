<template>


<section id="contact_section" class="d-flex justify-content-center">

 


    
 

    <div class="col-12 col-sm-6 col-md-4 mb-4 "  >
          <h1>Kontakt</h1>
      <form class="row g-3">
  <div class="col-md-12">
    <label for="inputEmail4" class="form-label">Email</label>
    <input type="email" class="form-control" placeholder="Email"  id="inputEmail4">
  </div>

<div class="input-group">

  <textarea class="form-control" placeholder="Skriv besked" aria-label="With textarea"></textarea>
</div>

 


  <div class="col-12">
    <button type="submit" class="btn btn-primary">Send</button>
  </div>
</form>
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
}
 
h1{color: #edf1f5 ;}

    

.active {
  background-color: khaki;
  
}
.text-color {
  color:darkviolet;
}
</style>
