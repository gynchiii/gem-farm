<template>
  <button class="button" :disabled="disabled">
    <img
      src="https://imagensemoldes.com.br/wp-content/uploads/2020/04/Arrow-PNG-1280x720.png"
      alt="right"
      :width="60"
      :height="60"
      :class="{ left: left, disabled: disabled }"
    />
  </button>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
  props: {
    left: Boolean,
    disabled: Boolean,
  },
  setup() {
    return {};
  },
});
</script>

<style scoped>
.button {
  color: white;
}
button,
img {
  outline: none !important;
  border-color: white;
  border: 1px;
}

.left {
  transform: scaleX(-1);
}
.disabled {
  opacity: 0;
}
</style>
