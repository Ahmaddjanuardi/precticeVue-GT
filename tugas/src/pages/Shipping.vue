<template>
  <div>
    <NavbarComponent></NavbarComponent>
    <BreadcrumbComponentVue></BreadcrumbComponentVue>
    <FormShippingVue></FormShippingVue>
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
    export default{
        name: 'ShippingPage',
        components: {
            NavbarComponent,
            BreadcrumbComponentVue,
            FormShippingVue,
            FooterComponentVue,
            CopyrightComponentVue
        }
    }
</script>

<style>

</style>