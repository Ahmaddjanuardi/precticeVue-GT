<template>
  <div id="app">
   <NavbarComponent> </NavbarComponent>
   <BreadcrumbComponentVue></BreadcrumbComponentVue>
   <GalleyComponentVue></GalleyComponentVue>
   <SliderComponentVue></SliderComponentVue>
   <FooterComponentVue></FooterComponentVue>
   <CopyrightComponentVue></CopyrightComponentVue>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import NavbarComponent from './components/NavabarComponent.vue';
import BreadcrumbComponentVue from './components/BreadcrumbComponent.vue';
import GalleyComponentVue from './components/GalleyComponent.vue';
import SliderComponentVue from './components/SliderComponent.vue';
import FooterComponentVue from './components/FooterComponent.vue';
import CopyrightComponentVue from './components/CopyrightComponent.vue';

export default {
  name: 'App',
  components: {
    NavbarComponent,
    BreadcrumbComponentVue,
    GalleyComponentVue,
    SliderComponentVue,
    FooterComponentVue,
    CopyrightComponentVue
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  /* margin-top: 60px; */
  
  
}
nav img{
    padding-left: 30px;
}
.nav-item{
    padding-right: 20px;
}
.breadcrumb{
    background-color: whitesmoke;
    padding: 10px;
}
.breadcrumb a{
    text-decoration: none;
    color: black;
}

.row .col-2 img{
    border-radius: 10px;
}
.row .col-6 img{
    border-radius: 20px;
}

.row .col-4 a{
    width: 50%;
    background-color: pink;
    border-radius: 30px;
    border: none;
}
.row .col-4 button img{
    padding: 10px;
}
.slide{
    padding: 6%;
}
footer .judul{
    text-align: center !important;
}
footer input{
    border-radius: 10px;
}

.input input{
    border: none;
}
.input button{
    background-color: rgb(245, 60, 60);
    width: 30px;
    height: 30px;
    border-radius: 5px;
    border: none;
}
footer{   
    background-color: white;
    color: black;
}
footer .footer{
    padding: 100px;
}
footer a{
    display: flex;
    align-items: center;
    text-decoration: none;
    padding: 0px;
    margin: 0px;
    color: black;
}
</style>
