<script>
import Tilt from 'vanilla-tilt-vue'

export default {
  name: 'App',
  components: {
    Tilt
  },
  data: function(){
    return {
      options: { gyroscope: true}
    }
  }
}
</script>

<template>
    <div class="buttons">           <div>
                <Tilt :options="options" parallax="true"> 
          <div class="container">
         <div class="wrapper">
           <div class="banner-image">
            <router-link to="/Acessorios" class="button" >Acessorios</router-link>
           </div>
          </div>
          
         
            </div></Tilt>
        </div>
        
              <div>  <Tilt :options="options" parallax="true">
          <div class="container">
         <div class="wrapper">
          
           <div class="banner-image">
            <router-link to="/marcas" class="button">Marcas</router-link> </div>
          
          </div>
          
            </div></Tilt>
        </div>
              
            </div>

            <div class="buttons">           <div>
                <Tilt :options="options" parallax="true"> 
          <div class="container">
         <div class="wrapper">
           <div class="banner-image">
            <router-link to="/Categorias" class="button">Categorias</router-link>
           </div>
          </div>
          
         
            </div></Tilt>
        </div>
        
              <div> <Tilt :options="options" parallax="true">
          <div class="container">
         <div class="wrapper">
          
           <div class="banner-image">
            <router-link to="/Cores" class="button">Cores</router-link> </div>
          
          </div>
          
            </div> </Tilt>
        </div>
              
            </div>
</template>

<style>
.wrapper{
    display: flex;
    align-items: end;
    }</style>