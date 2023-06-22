<template>
<h1>Notas: </h1>
<input type="text" name="" id="" v-model="note">

</template>

<script lang="ts" >
import { defineComponent,ref, watch } from "vue"
export default defineComponent({
  setup() {
    const note = ref("")
    watch(note, () => alert("se ha modificado el valor: " + note.value))
    return {
      note
    }
  }

})



</script>

<style>

</style>
