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
            <router-link to="/Acessorios">Acessorios</router-link>
           </div>
          </div>
          
          <div class="button-wrapper"> 
          <button class="btn outline">DETAILS</button>
          </div>
            </div></Tilt>
        </div>
        
              <div>  <Tilt :options="options" parallax="true">
          <div class="container">
         <div class="wrapper">
          
           <div class="banner-image"><router-link to="/marcas">Marcas</router-link> </div>
          
          </div>
          <div class="button-wrapper"> 
          <button class="btn outline">DETAILS</button>
          </div>
            </div></Tilt>
        </div>
              
            </div>

            <div class="buttons">           <div>
                <Tilt :options="options" parallax="true"> 
          <div class="container">
         <div class="wrapper">
           <div class="banner-image">
            <router-link to="/Categorias">Categorias</router-link>
           </div>
          </div>
          
          <div class="button-wrapper"> 
          <button class="btn outline">DETAILS</button>
          </div>
            </div></Tilt>
        </div>
        
              <div> <Tilt :options="options" parallax="true">
          <div class="container">
         <div class="wrapper">
          
           <div class="banner-image"><router-link to="/Cores">Cores</router-link> </div>
          
          </div>
          <div class="button-wrapper"> 
          <button class="btn outline">DETAILS</button>
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