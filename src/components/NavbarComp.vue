<template>
    <div class="main">
    <div class="nav1">
        <nav>
          <router-link to="/signup">Signup</router-link> |
          <router-link to="/login">Login</router-link> |
          <router-link to="/">Home</router-link> |
          <router-link to="/about">About</router-link> |
          <router-link to="/store">Store</router-link> |
          <router-link to="/productAdmin">product Admin</router-link> |
          <router-link to="/userAdmin">User Admin</router-link> |
           <router-link to="/editUser">Edit User</router-link> |
           <router-link to="/cart">Cart</router-link> |
          <router-link to="/contact">Contact</router-link> 
          
              <!-- <button v-if="$cookies.get('jwt')" @click="logout">Logout</button> -->
        </nav>
    </div>
    <div class="nav2">
        <svg id="cart" xmlns="http://www.w3.org/2000/svg" width="50" height="50" fill="currentColor" class="bi bi-cart-fill" viewBox="0 0 16 16">
          <path d="M0 1.5A.5.5 0 0 1 .5 1H2a.5.5 0 0 1 .485.379L2.89 3H14.5a.5.5 0 0 1 .491.592l-1.5 8A.5.5 0 0 1 13 12H4a.5.5 0 0 1-.491-.408L2.01 3.607 1.61 2H.5a.5.5 0 0 1-.5-.5M5 12a2 2 0 1 0 0 4 2 2 0 0 0 0-4m7 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4m-7 1a1 1 0 1 1 0 2 1 1 0 0 1 0-2m7 0a1 1 0 1 1 0 2 1 1 0 0 1 0-2"/>
        </svg>
    </div>
</div>
</template>
<script>
export default {
    
}
</script>
<style>
    .main {
        display:flex;
        text-align: center;
    }
    .nav1 {
        width : 80%;
        height: 10%;
    }
    .nav2 {
        width : 20%;
        height: 10%;
    }
#cart {

}
</style>