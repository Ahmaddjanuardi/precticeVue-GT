<template>
  <div class="card-body border-color-pink">
    <h5 class="card-title">Success!</h5>
    <p class="card-text">Your Data Has Been Submitted!</p>
    <router-link to="/detail" class="btn bg-color-pink text-dark">Back</router-link>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.border-color-pink{
    border: solid 2px pink;
}
.bg-color-pink{
    background-color: pink;
}
</style>