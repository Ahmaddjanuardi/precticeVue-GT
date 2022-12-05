<template>
  <div>
    <NavbarComponent></NavbarComponent>
    <BreadcrumbComponentVue></BreadcrumbComponentVue>
    <FormShippingVue></FormShippingVue>
    <SuccessFormVue class="d-none"></SuccessFormVue>
    <FooterComponentVue></FooterComponentVue>
    <CopyrightComponentVue></CopyrightComponentVue>
  </div>
</template>

<script>
    import NavbarComponent from '../components/NavabarComponent.vue';
    import BreadcrumbComponentVue from '../components/BreadcrumbComponent.vue';
    import FormShippingVue from '../components/FormShipping.vue';
    import FooterComponentVue from '../components/FooterComponent.vue';
    import CopyrightComponentVue from '../components/CopyrightComponent.vue';
    import SuccessFormVue from '@/components/SuccessForm.vue';
    export default{
        name: 'ShippingPage',
        components: {
            NavbarComponent,
            BreadcrumbComponentVue,
            FormShippingVue,
            FooterComponentVue,
            CopyrightComponentVue,
            SuccessFormVue
        },
    }
</script>

<style>

</style>