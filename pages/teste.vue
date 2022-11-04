<template>
  <Flicking :options="{ circular: true }" :plugins="plugins">
    <img src="~/assets/img/1.jpg" alt="" />
    <img src="~/assets/img/1.jpg" alt="" />
  </Flicking>
</template>

<script>
import { Flicking } from '@egjs/vue-flicking';
import { AutoPlay } from '@egjs/flicking-plugins';
export default {
  components: {
    Flicking,
  },
  data: () => {
    return {
      plugins: [
        new AutoPlay({ duration: 5000, direction: 'NEXT', stopOnHover: false }),
      ],
    };
  },
};
</script>

<style></style>
