<template>
  <div class="temp">
    <label for="nom">Longueur du rail </label>
    <br>
    <input type="text" name="nom" id="nom" />
  </div>
</template>

<script>
export default {
  name: "TextInput",
  props: {
    msg: String,
  },
};
</script>

<style>
</style>
