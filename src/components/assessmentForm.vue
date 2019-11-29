<template>
  <div>
    <form>
      <formHead />
      <names v-bind:students="students" />
      <input type="submit" value="Submit">
    </form>
  </div>
</template>


<script>
import formHead from './formHead.vue';
import names from './names.vue';

export default {
  name: 'assessmentForm',
  components: {
    formHead,
    names,
  },
   data() {
    return {
      students: [    
        { name: 'Kwabena Frimpong', class: '1A1', sex:'Male', id: 1},
        { name: 'Albert Frimpong', class: '1A1', sex:'Male', id: 2},
        { name: 'Attakora Jet', class: '1A1', sex:'Male', id: 3},
        { name: 'Emmanuel Frimpong', class: '1A1', sex:'Male', id: 4},
        { name: 'John Addai', class: '1A7', sex:'Male', id: 5},
        { name: 'Adwoa Manu', class: '1A2', sex:'Female', id: 6},
        { name: 'Emmanuel Kusi', class: '1S2', sex:'Female', id: 7},
        { name: 'Jasper Nuako', class: '1S4', sex:'Female', id: 8},
        { name: 'Bismark Oppong', class: '1S1', sex:'Male', id: 9},
      ]
    }
  },
}
</script>


<style scoped>
input[type="submit"]{
    margin-top: 2rem;
    margin-left: 40%;
    width: 8rem;
    height: 2rem;
    font-size: 1rem;
    font-style: italic;
    border-radius: 2%;
    text-align: center;
    background-color: blueviolet;
    color: #ffffff;
}

</style>
