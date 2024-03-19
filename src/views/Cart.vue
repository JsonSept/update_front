<template>
    <div>
        <table class="table table-striped">
                <tr>
                  <th class="">Product ID</th>
                  <th>Name</th>
                  <th>Description</th>
                  <th>price</th>
                  <th>Product</th>
                </tr>
                <tbody v-for="item in $store.state.products" :key="item">
                <td>{{item.prodID}}</td>
                <td>{{item.name}}</td>
                <td>{{item.description}}</td>
                <td>{{item.price}}</td>
                <td><img :src="item.image" alt="" height="80px" width="90px"></td>
                <td><button @click="deleteProduct(item.prodID)">Delete</button></td>
                <td><button @click="editProduct(item.prodID)">Edit</button></td>
            </tbody>
            
        </table>
    </div>
</template>
<script>
export default {
    
}
</script>
<style>
    
</style>