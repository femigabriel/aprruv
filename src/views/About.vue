<template>
  <div class="about">
    <Form2 v-show="current == 1" @previous="current = current - 1" />
  </div>
</template>
<script>
import Form2 from "@/components/Form2.vue";

export default {
  name: "About",
  components: {
    Form2,
  },

  data() {
    return {
      current: 1,
    };
  },
};
</script>

<style></style>
