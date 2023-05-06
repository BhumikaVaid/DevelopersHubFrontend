<template>
        <div  :class="developer.active ? 'active': 'nonactive' ">
            <h2>{{developer.name}}</h2>
        </div>
        
        <div>
        <div class='developer'>
        
        <br><h4>Skills</h4>{{developer.skills[0]}}, {{developer.skills[1]}}, {{developer.skills[2]}}, {{developer.skills[3]}}, {{developer.skills[4]}}, {{developer.skills[5]}}, {{developer.skills[6]}}, {{developer.skills[7]}}.<br>
        <br><h4>Email</h4> {{developer.email}}<br>
        <br><h4>Website</h4> {{ developer.website }}<br>
        <br><h4>YouTube</h4> {{developer.youtube}}<br>
        <br><h4>Based In</h4> {{developer.basedin}}<br>
        <br><h4>Joined</h4> {{developer.joined}}<br>
        
    </div>

    </div>
        
</template>

<script>

export default{
    name: 'SingleDeveloper',
    props:{
        developer: Array
    }
}
</script>

<style scoped>

.active{
    background-color: #005f73;
    color: whitesmoke;
}

.nonactive{
    background-color: #0a9396 !important;
}

h4{
    margin: 2px;
}

div{
    background-color: #219ebc;
    color: black;
    padding: 1em;
    text-align: center;
    width:80%;
    margin: auto;
    
}

.developer{
    background-color: #f1faee;
    color: black;
    text-align: left;
    width: 60%;
    margin: auto;

}



</style>