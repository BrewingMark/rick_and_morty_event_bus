<template lang="html">
  <div id="character-profile">
    <h2>{{character.name}}</h2>
    <img v-bind:src="character.image" alt="character image">
    <h4>Species: {{character.species}}</h4>
    <h4>Gender: {{character.gender}}</h4>
    <h4>Origin: {{character.origin.name}}</h4>
    <h4>Status: {{character.status}}</h4>
  </div>
</template>

<script>
export default {
  name: 'character-detail',
  props: ['character']
}
</script>

<style lang="css" scoped>

#character-profile {
  text-align: center;
  background-color: #97CE4C;
  border: solid 5px #f0e14a;
}

</style>
