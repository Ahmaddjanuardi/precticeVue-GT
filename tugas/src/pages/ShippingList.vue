<template>
  <div>
    <NavbarComponent></NavbarComponent>
    <BreadcrumbComponentVue></BreadcrumbComponentVue>
    <ShippingListTableVue></ShippingListTableVue>
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
export default {
    name: 'ShippingList',
    components: {
        NavbarComponent,
        BreadcrumbComponentVue,
        ShippingListTableVue,
        FooterComponentVue,
        CopyrightComponentVue
    },
}
</script>

<style>

</style>