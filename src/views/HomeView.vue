<template>

  <div class="home">
    <div>
    <!-- Your component content -->
    <div v-if="users">
      <p>Name: {{ users.name }}</p>
      <p>Email: {{ users.email }}</p>
      <!-- Display other user data as needed -->
    </div>
    <div v-else>
      <p>Loading user data...</p>
    </div>
  </div>
</div>


    
</template>




<script>
export default {
  computed: {
    user() {
      return this.$store.getters.getUserData;
    }
  },
  created() {
    this.$store.dispatch('fetchUser', 5);
  },
  data() {
    return {
      userID: 5 // Assuming you have a userId to fetch a specific user
    };
  }
}
</script>
