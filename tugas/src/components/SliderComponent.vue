<template>
  <div class="slide">
    <h3>Complate Your Room</h3>
    <h3>With What We Designed</h3>
    <!-- Ini yang pake for -->
    <div class="d-flex justify-content-between mt-4">
        <!-- <Card v-for="(item, index) in objCard" :key="index" :objCard="item">
           
        </Card> -->
        <Card v-for="(item, index) in arrCardTitle"
        :key="index" 
        :cardTitle="item"
        :cardPrice="arrCardPrice[index]" 
        :cardImage="arrCardImage[index]" @changePicture="changePictureFunc"></Card>
    </div>
    <!-- <div class="d-flex justify-content-between mt-4">
        <Card cardTitle="Saman Kakka"
            cardPrice="IDR 18.000.000"
            cardImage="chair-1" ></Card>
        <Card cardTitle="Saman Kakka"
            cardPrice="IDR 18.000.000"
            cardImage="chair-1" ></Card>
        <Card cardTitle="Saman Kakka"
            cardPrice="IDR 18.000.000"
            cardImage="chair-1" ></Card>
    </div> -->
  </div>
</template>

<script>
import Card from "./Card.vue"
export default {
name : "SlideComponent",
components : {
    Card
},
methods : {
    changePictureFunc : function(cardImage){
        this.$emit('changePicture', cardImage)
        //  alert(cardImage)
    }
},
data(){
    return{
        arrCardTitle : ["Cangkir Mauttie", "Saman Kakka", "Lino Dino", "Syail Ammeno"],
        arrCardPrice : ["89.300.000","14.500.000","22.000.000","12.000.000"],
        arrCardImage : ["chair-1","chair-2","chair-3","chair-4"]
    }
}
}
</script>

<style scoped>

</style>