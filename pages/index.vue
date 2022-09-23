<template>
  <div class="pb-20">
    <TheHeader />
    <main>
      <SectionUm />
      <SectionDois />
      <DermaAlergia />
    </main>
  </div>
</template>

<script>
import SectionUm from '../components/SectionUm.vue';
import TheHeader from '~/components/TheHeader.vue';
import SectionDois from '~/components/SectionDois.vue';
import DermaAlergia from '~/components/DermaAlergia.vue';

export default {
  name: 'IndexPage',
  components: { TheHeader, SectionUm, SectionDois, DermaAlergia },
};
</script>
