<template>
  <Button :link="whatsAppLink">
    <slot></slot>
  </Button>
</template>

<script>
import Button from "./Button.vue";

export default {
  props: {
    tel: {
      type: String,
      required: true,
    },
  },
  computed: {
    whatsAppLink() {
      return `https://wa.me/${this.tel}`;
    },
  },
  components: {
    Button,
  },
};
</script>
