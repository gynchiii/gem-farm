<template>
  <nav class="bg-nav text-aqua flex flex-row justify-center align-middle">
    <NavButton
      v-for="i in menu"
      :key="i.name"
      :title="i.name"
      :url="i.url"
      :class="{ active: path === i.url }"
    />
  </nav>
</template>

<script lang="ts">
import { defineComponent, computed } from 'vue';
import { useRoute } from 'vue-router';
import NavButton from '@/components/NavButton.vue';

export default defineComponent({
  components: { NavButton },
  setup() {
    const route = useRoute();
    const path = computed(() => route.path);

    const menu = [
      { name: '/', url: '/' },
      { name: 'FARM MANAGER', url: '/manager' },
      { name: 'FARMER', url: '/farmer' },
    ];

    return {
      menu,
      path,
    };
  },
});
</script>

<style scoped>
.text-aqua {
  color: rgb(172, 236, 213);
}
.bg-nav{
  background-color: rgb(18, 99, 72);
}


.more {
  @apply px-10 py-3 text-white
  hover:bg-black hover:text-white;
  outline: none;
}
</style>
