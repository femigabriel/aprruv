<template>
  <div class="home">
    <Form v-show="current == 0" @next="current = current + 1" />
  </div>
</template>

<script>
// @ is an alias to /src
import Form from "@/components/Form.vue";

export default {
  name: "Home",
  components: {
    Form,
  },
  data() {
    return {
      current: 0,
    };
  },
};
</script>
