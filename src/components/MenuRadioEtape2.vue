<template>
  <div class="temp">
    <div>
      <input type="radio" id="masculin" name="sexe" value="masculin" checked />
      <label for="masculin">Modèle DS : Fiaxation au plafond pour rideaux légers (sans doublure, hauteur max 300com)</label>
    </div>
    <div>
      <input type="radio" id="feminin" name="sexe" value="feminin" />
      <label for="feminin">Modèle CS : Fixation au plafond pour rideaux lourds (doublé, hauteur + 300 cm)</label>
    </div>
  </div>
</template>

<script>
export default {
  name: "MenuRadioEtape2",
  props: {
    msg: String,
  },
};
</script>

<style>
</style>