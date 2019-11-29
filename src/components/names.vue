<template>
    <div id="names">
        <div id="nameHead"> <p>Names of Students</p><p>Marks</p> </div>
        <div id="name" v-for="student in students" v-bind:key="student">
           <p>{{student.name}}</p><p><input type="text" name="" id=""></p>
        </div>
    </div>
</template>



<script>
export default {
    name: 'name',
    props: ["students"],
}
</script>



<style scoped>
#names {
    text-align: left;
    width: 80%;
    margin-left: 10%;
    margin-top: 2rem;
}

#name {
    display: grid;
    grid-template-columns: 60% 40%;
    margin-top: 0.5rem;
}

#nameHead {
    display: grid;
    grid-template-columns: 60% 40%;
    font-weight: bold;
    font-size: 20px;
}

input[type="text"]{
    width: 8rem;
    height: 1.5rem;
}



</style>