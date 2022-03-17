<template>
  <div class="about">
    <Form2 />
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
      current: 0,
    };
  },

  methods: {
    previous() {
      // this.current = this.current - 1;
      this.$emit("previous");
    },
  },
};
</script>

<style></style>
