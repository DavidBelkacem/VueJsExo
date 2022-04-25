<template>
  <div class="cityComponent">
      <p>  Ville : {{ name }} </p>
      <p>  Temps : {{ weather}} </p>
      <p>  Temperature : {{ temperature }} </p>
      <p>  Mis à jour : {{ timeSinceUpdate }} </p>
    </div>
</template>
  
<script>
  import * as timeago from 'timeago.js';

  export default {
    name: "CityComponent",
    props: {
      name: String,
      weather: String, 
      temperature : Number,
      updatedAt : Date,
      },
    computed : {
      timeSinceUpdate: function() {
        return timeago.format(this.updatedAt)
      }
    },
  };
</script>

<style scoped>
  .cityComponent {
    margin: 80px;
    border : solid 3px;
    width:400px;
  }
</style>
