<template>
    <h1 :style="{color:colorie}">Tringle Rail</h1>
<img src="https://cdn2.mesrideaux.fr/media/catalog/product/cache/c4f8953d6b68b8073272b21c1e15595e/t/r/tringles-rail.jpg">
   
      <div v-if="step === 'step1'">
      <h1>1 : J'indique mes dimentions</h1>
      <TextInput msg="" />
    <ChangeColor msg="" v-on:validation="step='step2'"/>
    </div>
    <div v-if="step === 'step2'">
      <h1>2 : J'indique mon type de rail</h1>
      <MenuRadioEtape2 msg="" />
    <ChangeColor msg="" v-on:validation="step='step3'"/>
    </div>
    <div v-if="step === 'step3'">
      <h1>3 : Je sélectionne mes supports</h1>
       <MenuRadioEtape3 msg="" />
        <ChangeColor msg="" v-on:validation="step='step4'"/>
    <div v-if="step === 'step4'">
        <Confirmation msg=""/>
          <ChangeColor msg="" v-on:validation="step='step4'"/>
   </div>

    </div>
</template>

<script>
import TextInput from "./components/TextInput.vue";
import MenuRadioEtape2 from "./components/MenuRadioEtape2.vue";
import MenuRadioEtape3 from "./components/MenuRadioEtape3.vue";
import ChangeColor from "./components/ChangeColor.vue";
import Confirmation from "./components/Confirmation.vue";

export default {
  name: "App",
  components: {
    TextInput,
    MenuRadioEtape2,
    MenuRadioEtape3,
    ChangeColor,
    Confirmation,
  },
  data() {
    return {
      colorie: 'red',
      step: 'step1'
    }
  }
};
</script>

<style>
.temp {
  margin: 1em;
}
</style>