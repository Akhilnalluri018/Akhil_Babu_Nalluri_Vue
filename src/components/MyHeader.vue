<template>
    <div id="home" class="Navigation">
        <nav class="navbar">
            <h1>TOP COUNTRIES IN THE WORLD AND THEIR STATISTICS</h1>
               </nav>
    </div>
    </template>
    
    <script>
    
    export default{
        name:'MyHeader',
        methods:{
            onClick(){
                console.log("We just clicked")
            }
        }
    }
    
    </script>
    <style scoped>
    .Navigation{
        size: 1vmax;
    }
    li {
     list-style: none;
    }
    .navbar {
    margin-left: auto;
    margin-right: auto;
    /* align-items: center; */
     padding: 15px;
     background-color: rgb(173, 192, 152);
     color: rgb(0, 0, 0);
     font-size: 42px;

    }  
    </style>
    