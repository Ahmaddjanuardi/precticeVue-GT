<template>
    <div>
<h1>Table List</h1>
<table class="table">
<thead>
  <tr>
    <th scope="col">No</th>
                    <th scope="col">ID</th>
                    <th scope="col">Nama</th>
                    <th scope="col">Email</th>
                    <th scope="col">Phone Number</th>
                    <th scope="col">City</th>
                    <th scope="col">Alamat</th>
                    <th scope="col">Postal Code</th>
                    <th scope="col">Action</th>
  </tr>
</thead>
<tbody>
    <tr v-for="(item, index) in shippingData" :key="item.id">
                    <th>{{ index + 1 }}</th>
                    <td>{{ item.id }}</td>
                    <td>{{ item.first_name + " " + item.last_name }}</td>
                    <td>{{ item.email }}</td>
                    <td>{{ item.phone_number }}</td>
                    <td>{{ item.city }}</td>
                    <td>{{ item.address }}</td>
                    <td>{{ item.postal_code }}</td>
  </tr>
</tbody>
</table>
    </div>
</template>

<script>
// import ShippingList from '@/pages/ShippingList.vue';
import shippingService from '@/service/shippingService';
export default {
methods:{
  getShipping(){
    shippingService.getAll()
    .then(response => {
        this.shippingData = response.data
        console.log(this.shippingData);
        //this.success = true;
      }).catch(e =>{
        console.log(e)
      });
  },
  mounted(){
    this.getShipping();
  },
  data(){
    return{
        shippingData : null,
    }
  }
}
}
</script>

<style>

</style>