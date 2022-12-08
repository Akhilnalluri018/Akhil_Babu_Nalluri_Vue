<template>
  
  <MyHeader />
  <CountryBox :countries="countries" />
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import CountryBox from './components/CountryBox.vue'


export default {
  name: 'App',
  components: {
    MyHeader,
    CountryBox
  },
  data(){
    return {
      countries: []
    }
  },
  methods: {
    // promises

      async fetchCountries(){
         const res= await fetch('http://localhost:4107/api')
         const data= await res.json()
          console.log(data)
         return data
      }

  },

  async created(){
    this.countries = await this.fetchCountries()
  }
}

</script>

<style>
#app {
  
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    color: black;
}
</style>
