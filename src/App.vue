<template>
  <div id="app" class="h-100">
    <div class="container-fluid h-100">
      <div class="row h-100">
        <div class="col-md-3 vue-bg h-100 d-flex justify-content-center align-items-center">
         <nav class="nav flex-column">
            <a class="nav-link active" href="#">
              <svg xmlns="http://www.w3.org/2000/svg" width="50" height="50" fill="currentColor" class="bi bi-person-circle" viewBox="0 0 16 16">
                <path d="M11 6a3 3 0 1 1-6 0 3 3 0 0 1 6 0z"/>
                  <path fill-rule="evenodd" d="M0 8a8 8 0 1 1 16 0A8 8 0 0 1 0 8zm8-7a7 7 0 0 0-5.468 11.37C3.242 11.226 4.805 10 8 10s4.757 1.225 5.468 2.37A7 7 0 0 0 8 1z"/>
              </svg>
            </a>
            <a class="nav-link active" href="#">Meu perfil</a>
            <a class="nav-link active" href="#">Cadastros</a>
            <a class="nav-link active" href="#">Novo</a>
            <a class="nav-link active" href="#">Atalhos</a>
            <a class="nav-link" href="#">Configurações</a>
            <a class="nav-link" href="#">Sair</a>
          </nav>
        </div>
        <div class="col-md-9 h-100 d-flex  justify-content-center align-items-center"> 
          <!-- <button id="bt-novo" type="button" class="btn btn-success btn-sm">
            <svg xmlns="http://www.w3.org/2000/svg" width="10" height="16" fill="currentColor" class="bi bi-plus-lg " viewBox="0 0 16 16">
              <path d="M8 0a1 1 0 0 1 1 1v6h6a1 1 0 1 1 0 2H9v6a1 1 0 1 1-2 0V9H1a1 1 0 0 1 0-2h6V1a1 1 0 0 1 1-1z"/>
            </svg>
              Novo</button> -->
          <div class="col-md-10 rounded px-5 py-4 shadow bg-white text-left">
            <SignupForm />
          </div>
        </div>
      </div>
        <!-- <p>©Copyright 2050 by nobody. All rights reversed.</p> -->
    </div>
   

  </div>
 
</template>

<script>
import SignupForm from './components/SignupTable.vue'

export default {
  name: 'App',
  components: {
    SignupForm
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.vue-bg {
  background: #39F;
  position: relative;
}

.nav-link{
  font-family:Arial, Helvetica, sans-serif;
  color: whitesmoke;
  position: relative;
}

.navbar{
  max-height: 70px;
  background: white;
  margin-left: 25%;
}

#bt-novo{
 padding-right: 50px; 
 

 position: relative;
 bottom: 43%;
 left: 0%;
}

.bi{
  color: aliceblue;
}

.col-md-10{
 position: relative;
 

right: 4%;
}

tr,th{
  font-size: 15px;
}

table{
   max-height: 35vh;
  
}


</style>
