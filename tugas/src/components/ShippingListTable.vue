<template>
    <div>
        <h1 class="text-center my-5">Shipping List</h1>
        <table class="table table-striped">
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
                        <td class="d-flex">
                            <button class="btn btn-sm btn-warning mr-2 text-white" @click="$emit('updateShippingFunc', item)">Update</button>
                            <button class="btn btn-sm btn-danger mr-2" @click="deleteShippingFunc(item.id)">Delete</button>
                        </td>
                    </tr>
                </tbody>
        </table>
    </div>
</template>

<script>
// import ShippingList from '@/pages/ShippingList.vue';
import shippingService from '@/service/shippingService';
export default {
    methods : {
        getShipping(){
            shippingService.getAll()
                .then(response => {
                    this.shippingData = response.data;
                    console.log(this.shippingData);
                })
                .catch(e => {
                    console.log(e);
                });
        },
        deleteShippingFunc(id){
            if (confirm("Apakah anda yakin ingin menghapus data ini?")) {
                shippingService.deleteShipping(id)
                .then(response => {
                    console.log(response.data)
                })
                .catch(e =>{
                    console.log(e);
                });
            } else {
                alert("Hapus Dibatalkan!")
            }
        }

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
</script>

<style>

</style>