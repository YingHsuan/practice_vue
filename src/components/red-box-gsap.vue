<template>
  <div ref="box" class="box"></div>
</template>

<script>
import { TimelineLite } from "gsap";
export default {
  mounted() {
    const { box } = this.$refs;
    const timeline = new TimelineLite();

    timeline.to(box, 1, { x: 200, rotation: 90 });
  }
};
</script>

<style>
/* styles emitted */
</style>