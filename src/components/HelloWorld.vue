<template>
  <div id="HelloWorld">
    <CityComponent 
      :name="name"
      :weather="weather"
      :temperature="temperature"
      :updatedAt="updatedAt"/>
  </div>
</template>

<script>
  import CityComponent from "./City.vue";

  export default {
    name: "HelloWorld",
    data() {
      return {
        name: "Ma ville", // nom de la ville
        weather: "Peu nuageux", // descriptif météo
        temperature: 20.55, // température en °C
        updatedAt: new Date(), // date de dernière mise à jour
      }
    },
    components: {
      CityComponent,
    },
  };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
