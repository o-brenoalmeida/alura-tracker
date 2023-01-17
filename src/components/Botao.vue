<template>
    <button class="button" @click="$emit('acao')">
      <span class="icon">
        <i :class="icone"></i>
      </span>
      <span>{{ texto }}</span>
    </button>
    
</template>

<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
  name: "Botao",
  props: {
    texto: {
        type: String,
        default: "play"
    },
    icone: {
        type: String,
        default: "fas fa-play"
    }
  }
  
});
</script>