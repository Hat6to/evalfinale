<template>
  <div class="temp">
    <div>
      <input type="radio" id="masculin" name="sexe" value="masculin" checked />
      <label for="masculin">Blanc</label>
    </div>
    <div>
      <input type="radio" id="feminin" name="sexe" value="feminin" />
      <label for="feminin">Noir</label>
    </div>
  </div>
</template>

<script>
export default {
  name: "MenuRadioEtape3",
  props: {
    msg: String,
  },
};
</script>

<style>
</style>