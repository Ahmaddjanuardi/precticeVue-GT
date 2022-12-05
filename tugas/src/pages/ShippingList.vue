<template>
  <div>
    <NavbarComponent></NavbarComponent>
    <BreadcrumbComponentVue></BreadcrumbComponentVue>
    <div class="row justify-content-center">
      <div class="col-10">
        <ShippingListTableVue v-show="!viewForm" @updateShippingFunc="updateShippingFunc"></ShippingListTableVue>
        <FormShippingVue v-show="viewForm" :shippingDataProps="shippingData"></FormShippingVue>
      </div>
    </div>
    <FooterComponentVue></FooterComponentVue>
    <CopyrightComponentVue></CopyrightComponentVue>
  </div>
</template>

<script>
    import NavbarComponent from '../components/NavabarComponent.vue';
    import BreadcrumbComponentVue from '../components/BreadcrumbComponent.vue';
    import ShippingListTableVue from '../components/ShippingListTable.vue';
    import FooterComponentVue from '../components/FooterComponent.vue';
    import CopyrightComponentVue from '../components/CopyrightComponent.vue';
    import FormShippingVue from '@/components/FormShipping.vue';
export default {
    name: 'ShippingList',
    components: {
        NavbarComponent,
        BreadcrumbComponentVue,
        ShippingListTableVue,
        FooterComponentVue,
        CopyrightComponentVue,
        FormShippingVue
    },
    methods:{
        updateShippingFunc(item){
          this.shippingData = item
          this.viewForm = true;
        }
      },
        data(){
          return{
            viewForm : false,
            shippingData : null
          
        }
      }
}
</script>

<style>

</style>