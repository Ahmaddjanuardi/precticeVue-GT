<template>
    <div>
        <nav class="breadcrumb">
        <router-link to="/detail" class="breadcrumb-item" >Home</router-link>
        <router-link to="/detail" class="breadcrumb-item" >Detail</router-link>
        <router-link to="/shipping" class="breadcrumb-item" v-show="breadlink == '/shipping'"> Shipping</router-link>
      </nav>
    </div>
</template>

<script>
export default {
  name: 'breadcrumbView',
  data(){
    return {
      breadlink : this.$route.path
    }
  }
}
</script>

<style lang="scss" scoped>

</style>
