<template>
  <div>
    <TheHeader />
    <main>
      <SectionUm />
      <SectionDois />
      <DermaAlergia />
      <BanhoTosa />
      <HotelSection />
      <CrecheSection />
      <CursosSection />
      <FotosSection />
    </main>
    <TheFooter />
  </div>
</template>

<script>
import SectionUm from '../components/SectionUm.vue';
import TheHeader from '~/components/TheHeader.vue';
import SectionDois from '~/components/SectionDois.vue';
import DermaAlergia from '~/components/DermaAlergia.vue';
import BanhoTosa from '~/components/BanhoTosa.vue';
import HotelSection from '~/components/HotelSection.vue';
import CrecheSection from '~/components/CrecheSection.vue';
import TheFooter from '~/components/TheFooter.vue';
import CursosSection from '~/components/CursosSection.vue';
import FotosSection from '~/components/FotosSection.vue';

export default {
  name: 'IndexPage',
  components: {
    TheHeader,
    SectionUm,
    SectionDois,
    DermaAlergia,
    BanhoTosa,
    HotelSection,
    CrecheSection,
    TheFooter,
    CursosSection,
    FotosSection,
  },
};
</script>
