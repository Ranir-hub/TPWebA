<script setup>
import Vheader from "./assets/components/Vheader.vue";

import Vpromo from "./assets/components/Vpromo.vue";
import Vteacher from "./assets/components/Vteacher.vue";
import Vlesson from "./assets/components/Vlesson.vue";
import Vpossibility from "./assets/components/Vpossibility.vue";
import Vhow from "./assets/components/Vhow.vue";
import Vdistance from "./assets/components/Vdistance.vue";

import Vfooter from "./assets/components/Vfooter.vue";
</script>

<template>
  <div class="body_wraper">
    <vheader/>
  </div>

    <main>
      <vpromo/>
      <vteacher/>
      <vlesson/>
      <vpossibility/>
      <vhow/>
      <vdistance/>
    </main>

    <vfooter/>
</template>

<style scoped>

</style>
