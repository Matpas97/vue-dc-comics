
<!-- Template -->
<template>
    <main>
   <div class="content">MAIN CONTENT GOES HERE </div> 






    </main>
</template>


<!-- Scriptc-->
<script>
    export default {
        name:"MainComponent",

    }




</script>

<!-- Style -->
<style lang="scss" scoped>
 @import '@/styles/variables.scss';

main {
    background-color: $bg-main;
    height: 150px;
   
    
}
.content {
    text-align: left;
    color: white;
    margin: 0 auto;
    width: 75%;
   padding-top: 50px;
}



</style>