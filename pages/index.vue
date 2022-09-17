<template>
  <div>
    <TheHeader />
    <main>
      <SectionUm />
    </main>
  </div>
</template>

<script>
import SectionUm from '../components/SectionUm.vue';
import TheHeader from '~/components/TheHeader.vue';

export default {
  name: 'IndexPage',
  components: { TheHeader, SectionUm },
};
</script>
