<template>
  <div id="bloqueCasinoApuesta">
    <v-img src="@/assets/images/fondito_final.jpg" style="position:sticky;">
      <img
        class="mt-12"
        data-aos="flip-left"
        data-aos-duration="2000"
        data-aos-once="true"
        id="imageLogo"
        src="@/assets/images/logo.png"
        alt
      />
    </v-img>
  </div>
</template>

<script>
export default {
  name: "bloqueCasinoApuesta",
};
</script>

<style>
#imageLogo {
  width: 30%;
}

#bloqueCasinoApuesta {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>