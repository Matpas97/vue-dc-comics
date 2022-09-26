<!-- Template -->
<template>
    <header>
        <!-- Logo Left -->
        <div class="logo-left">
            <img src="../assets/img/dc-logo.png" alt="logo png">
        </div>
        <!-- List right  Nav -->
      <nav>
        <ul>
            <li v-for="(element,index) in navElements" :key="index" >
              <a :href="element.link" :class="{active: element.active}" >
                 {{ element.name }}
               </a></li>
        </ul>
      </nav>




    </header>
 </template>
 


 <!-- Script -->
 <script>
export default {
    name:"MainHeader",
    data () {
        return {
            navElements:[
                {
                    name:"CHARACTERS",
                    link:"#",
                    active:true
                },
                {
                    name:"COMICS",
                    link:"#",
                    active:false
                },
                {
                    name:"MOVIES",
                    link:"#",
                    active:false
                },
                {
                    name:"TV",
                    link:"#",
                    active:false
                },
                {
                    name:"COLLECTIBILES",
                    link:"#",
                    active:false
                },
                {
                    name:"VIDEOS",
                    link:"#",
                    active:false
                },
                {
                    name:"FANS",
                    link:"#",
                    active:false
                },
                {
                    name:"NEWS",
                    link:"#",
                    active:false
                },
                {
                    name:"SHOP",
                    link:"#",
                    active:false
                }
            ],
        }
    
    }
}
 </script>

 <!-- Style  -->
 <style lang="scss" scoped>
    @import '../styles/variables.scss';
    header {
        display: flex;
        justify-content: space-between;
        margin: 0 auto;
        width: 75%;
    }
    
    ul {
        display: flex;
        vertical-align: middle;
        height: 100%;
       
       
    }
    li {
        list-style-type: none;
        padding: 0 15px;
        height: 100%;
       
       
    }
    .logo-left img {
        vertical-align: middle;
    }
    a {
        text-decoration: none;
        color: #000;
        height: 60px;
        display: flex;
        text-transform: uppercase;
        &.active {
            border-bottom: 5px solid #0082f9;

        }
    }
  

    
 </style>
