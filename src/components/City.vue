<template>
  <div class="cityComponent">
    <p>  Ville : {{ name }} </p>
    <p>  Temps : {{ weather}} </p>
    <p>  Temperature : {{ temperature }} </p>
    <p>  Mis à jour : {{ updatedAt }} </p>
  </div>
</template>
  
<script>
  export default {
    name: "cityComponent",
    props: {
      name: String,
      weather: String, 
      temperature : Number,
      updatedAt : Date
      }
  };
</script>
