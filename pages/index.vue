<template>
  <div>
    <TheHeader />
    <main>
      <SectionUm />
      <SectionDois />
    </main>
  </div>
</template>

<script>
import SectionUm from '../components/SectionUm.vue';
import TheHeader from '~/components/TheHeader.vue';
import SectionDois from '~/components/SectionDois.vue';

export default {
  name: 'IndexPage',
  components: { TheHeader, SectionUm, SectionDois },
};
</script>
