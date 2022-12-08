<template>
    <td>{{country.Rank}}</td>
    <td>{{country.Country}}</td>
    <td>{{country.Capital}}</td>
    <td>{{country.Population}}</td>
    <td>{{country.GDP}}</td>
    <td>{{country.Percapitaincome}}</td>
    <td>{{country.Area}}</td>
    <td>{{country.Currency}}</td>
    <td>{{country.Famousfor}}</td>
    </template>
    
    <script>
    
    export default{
        name: 'SingleCountry',
        props:{
            country: Array
        }
    }
    </script>
    
    <style scoped>
    td{
        padding: 20px;
        border: 3px solid rgb(0, 0, 0);
    }
    </style>