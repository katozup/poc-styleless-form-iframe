<template>
  <div class="formulary-wrapper">
    <Formulary />
  </div>
</template>

<script>
// @ is an alias to /src
import Formulary from '@/components/Formulary.vue';

export default {
  name: 'FormPage',
  components: {
    Formulary,
  },
};
</script>
