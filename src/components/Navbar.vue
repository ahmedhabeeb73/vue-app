<template>
  <div class="navbar">
  <nav class="nav-extended">
    <div class="nav-content">
      <router-link to="">
        <span class="nav-title">Vue app</span>
      </router-link>

      <a title="add" href="" class="btn">
        <router-link to="">
          <i class="fas fa-plus"></i>
        </router-link>
      </a>
    </div>

  </nav>
  </div>
</template>


<script>
export default {
  name:"Navbar",
  data(){
    return {

    }
  }
}
</script>

<style>
body {
  background:#ccc;
}
*{
  padding: 0;
  margin:0;
  box-sizing: border-box;
}
html {
  font-size: 62.5%;
}

.nav-extended{
  background:blue;
}
a {
  text-decoration:none;
}

.nav-content {
 
 display: flex;
justify-content: space-between; 
padding:2rem;
justify-items: center;


}

.nav-title{
  color:#fff;
  font-size: 3rem;
}

.btn {
  display:inline-block;
  background:red;
  color:#fff;
  padding:30px ;
  border-radius: 50%;
   margin-top:1rem;
 
  
}
.fas{
  color:#fff;
  font-size:20px;
  
  
}

</style>