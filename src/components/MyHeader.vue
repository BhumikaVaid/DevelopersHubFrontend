<template>
    <div>
        <h1> {{appName}} </h1>
        <h4>- {{yourName}} </h4>        
    </div>

    
    </template>
    
    <script>
    
    export default{ // Exporting Default Object
        name: 'MyHeader',
        props:{ 
    
            appName:String,
            yourName: String
        }
    }
    
    </script>
    
    <style scoped>
    
    
    div{
        background-color: #001d3d;
        color: whitesmoke;
        padding: 1em;
        text-align: center;
        width: 80%;
        margin: auto;
    }
    
    </style>