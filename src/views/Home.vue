<template>
  <div>
    <app-header></app-header>
  </div>
</template>

<script lang="ts">
  import { defineComponent } from 'vue';
  import AppHeader from '@/components/AppHeader.vue';

  export default defineComponent({
    name: 'Home',
    components: {
      AppHeader,
    },
  });
</script>
