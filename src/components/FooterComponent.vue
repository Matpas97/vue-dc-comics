

<!-- Template -->
<template>
    <div>
    <ShopFooterContent/>
    <InfoFooterContent/>
    <LoginFooterContent/>


    </div>
</template>


<!-- Script -->
<script>
    import ShopFooterContent from './ShopFooterContent.vue';
    import InfoFooterContent from './InfoFooterContent.vue';
    import LoginFooterContent from './LoginFooterContent.vue';


    export default {
        name:'FooterComponent',
        components: {
    ShopFooterContent,
    InfoFooterContent,
    LoginFooterContent,
   },
      
        };
    




</script>


<!-- Style -->
<style lang="scss" scoped>





</style>