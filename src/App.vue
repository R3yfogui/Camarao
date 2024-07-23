<script setup>
import { onMounted } from 'vue';
import { PassageUser } from '@passageidentity/passage-elements/passage-user';
import { useAuthStore } from '@/stores/auth';

    

const authStore = useAuthStore();

</script>

<template>
  
    
    <div v-if="authStore.loggedIn">
      <div class="topnav">
  <a class="active" href="#home"><router-link :to="{ name: 'home' }">Home</router-link> </a>
  <a><router-link  to="/logout">Logout</router-link> </a> 
  <a href="">{{ authStore.user.email }}</a>
</div>
     
      
    </div>
    
    <router-link v-else to="/login">Login</router-link>
  
  <main>
    <RouterView />
  </main>

  
  
  
</template>

<style>
.topnav {
  background-color: #333;
  overflow: hidden;
}

/* Style the links inside the navigation bar */
.topnav a {
  float: left;
  color: #f2f2f2;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
}

/* Change the color of links on hover */
.topnav a:hover {
  background-color: #ddd;
  color: black;
}

/* Add a color to the active/current link */
.topnav a.active {
  background-color: #04AA6D;
  color: white;
}
</style>