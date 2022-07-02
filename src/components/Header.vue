<template>
  <div class="py-4">
    <h2 class="font-bold text-2xl text-white md:text-4xl" v-html="text"></h2>
  </div>
</template>

<script>
export default {
  name: "HeaderComp",
  props: ["text"],
};
</script>
