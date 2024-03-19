<template>
  <navbar-comp/>
  <router-view/>
  <!-- <spinner/> -->
  <footer-comp/>
</template>

<script>
// import Spinner from './components/Spinner.vue';
import NavbarComp from './components/NavbarComp.vue';
import FooterComp from './components/FooterComp.vue';


export default {
  components: {
    NavbarComp,
    FooterComp,
    // Spinner,
  }
}


</script>


<style>

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fafafa;
  padding-bottom: 70%;
  /* background-image: url('https://i.ibb.co/2qV7YLd/wp4006828.jpg'); */
  background-color:darkblue;
  background-repeat: no-repeat;
  background-size: cover;
  
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #f7f8fa;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
