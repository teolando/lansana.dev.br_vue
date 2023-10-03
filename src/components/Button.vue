<template>
  <a :href="link" class="button"><slot></slot></a>
</template>

<script>
export default {
  props: {
    link: {
      type: String,
      required: true,
    },
  },
};
</script>

<style>
.button {
  height: 70px;
  width: 300px;
  line-height: 70px;
  text-decoration: none;
  color: white;
  text-align: center;
  border-radius: 30px;
  background-color: #0d7377;
  margin-bottom: 30px;
}

@media only screen and (max-width: 600px) {
  .button {
    width: 240px;
    height: 60px;
    line-height: 60px;
    font-size: 16px;
  }
}

@media only screen and (min-width: 1200px) {
  .button {
    height: 70px;
    width: 300px;
  }
}
</style>
