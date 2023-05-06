<template>
   
    
    <div v-for="developer of developers" :key="developer.developerid" >

     
       <SingleDeveloper :developer=developer />

    </div>

</template>
<script>
import SingleDeveloper from './SingleDeveloper.vue'

export default {
    name: 'DevelopersBox',
    props:{
        developers: Array
    },
    components:{
        SingleDeveloper
    }
    
}
</script>
<style scoped>

</style>
