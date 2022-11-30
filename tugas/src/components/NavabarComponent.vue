<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-danger">
       <div class="container-fluid">
         <img src="../assets/img/logo.png" alt="logo" />
         <button
           class="navbar-toggler"
           type="button"
           data-bs-toggle="collapse"
           data-bs-target="#navbarSupportedContent"
           aria-controls="navbarSupportedContent"
           aria-expanded="false"
           aria-label="Toggle navigation"
         >
           <span class="navbar-toggler-icon"></span>
         </button>
         <div class="d-flex justify-content-between" id="navbarSupportedContent">
           <ul class="navbar-nav ms-auto">
             <li class="nav-item">
               <router-link to="/shipping" class="nav-link" aria-current="page">Shipping</router-link>
             </li>
             <li class="nav-item">
               <a class="nav-link" href="#">Catalog</a>
             </li>
             <li class="nav-item">
               <a class="nav-link" href="#">Delivery</a>
             </li>
             <li class="nav-item">
               <a class="nav-link" href="#">Rewards</a>
             </li>
             <li class="nav-item pt-1">
               <a href="nav-item">
                 <img src="../assets/img/cart3.svg" alt="" />
               </a>
             </li>
           </ul>
         </div>
       </div>
     </nav>
</template>

<script>
export default {
  name: 'NavbarComponentView',
}
</script>

<style scoped>

</style>