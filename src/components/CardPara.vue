<template>
  <div>
    <p>{{ paraMessage }}</p>
  </div>
</template>

<script>
export default {
  props: {
    paraMessage: String,
  },
};
</script>

<style scoped>
p {
  font-size: 15px;
  text-align: center;
  padding: 5px 35px 30px 35px;
}
</style>