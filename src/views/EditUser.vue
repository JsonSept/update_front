<template>
    <div>
        <div>
            
        <input type="firstname" firstname="firstname" placeholder="firstname" v-model="firstname"><br><br>
        <input type="lastname" lastname="lastname" placeholder="lastname" v-model="lastname"><br><br>
        <input type="email" name="email" placeholder="email" v-model="email"><br><br>
        <input type="password" name="password" placeholder="password" v-model="password"><br><br>
        <button @click="editUser">Save Changes</button>
        <!-- {{ $store.state.loggedIn }}
        <button @click="loginUser">Login</button> -->
    </div>
    </div>
</template>
<script>
export default {
    data(){
        return {
            firsname:null,
            lastname:null,
            email:null,
            password:null
        }
    },
    methods : {
        editUser(){
            console.log(this.$data);
            this.$store.dispatch(this.$data)
        }
    }
}
</script>
<style>
    
</style>