  <script>
    export default {
    name: "CityTest",
    // props: {
    //   msg: String,
    // },
    data() {
      return {
        name: "Ma ville", // nom de la ville
        weather: "Peu nuageux", // descriptif météo
        temperature: 20.55, // température en °C
        updatedAt: new Date(), // date de dernière mise à jour
      }
    },
  };
</script>
