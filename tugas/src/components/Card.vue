<template>
    <div class="bg-white p-4 border-radius-25">
        <div class="card p-3" style="width: 18rem; padding: 30px ;">
            <a href="#" @click.prevent="$emit('changePicture', cardImage)" class="chairs">
                <img class="border-radius-25" 
                :src="require('@/assets/img/' + cardImage + '.png')" alt="chair">
            </a>
            <p class="font-weight-bold mt-3 my-0">{{cardTitle}}</p>
            <p>IDR{{cardPrice}}</p>
        </div>
    </div>
</template>

<script>
export default {
name : "CardComponent",
props : ["cardTitle", "cardPrice", "cardImage"]
}
</script>

<style scoped>
</style>