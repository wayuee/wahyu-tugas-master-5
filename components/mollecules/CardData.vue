<template>
  <div class="float-right pt-5 pb-8 px-14 bg-blue-200 pb-16 rounded-xl">
    <h1 class="text-xl font-bold text-center">Registration Data</h1>
    <InputText labelInput="Firstname" :input-value="CardData.fnameR" v-model="CardData.fnameR" />
    <InputText labelInput="Lastname" :input-value="CardData.lnameR" v-model="CardData.lnameR" />
    <InputText labelInput="Gender" :input-value="CardData.genderR" v-model="CardData.genderR" />
    <InputText labelInput="Email" :input-value="CardData.emailR" v-model="CardData.emailR" />
    <InputText labelInput="NumberPhone" :input-value="CardData.numberR" v-model="CardData.numberR" />
    <InputText labelInput="Adress" :input-value="CardData.adressR" v-model="CardData.adressR" />
    <InputText labelInput="PostalCode" :input-value="CardData.postalR" v-model="CardData.postalR" />
  </div>
</template>

<script>
import InputText from "~/components/atoms/InputText";
export default {
  components: {
    InputText,
  },
  props:{
    CardData:{
      type:Object,
      default:{}
    }
  },
};
</script>

<style></style>
