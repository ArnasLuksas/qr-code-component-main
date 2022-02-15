<template>
  <div>
    <h1>{{ titleMessage }}</h1>
  </div>
</template>


<script>
export default {
  props: {
    titleMessage: String,
  },
};
</script>
<style scoped>
h1 {
  font-size: 25px;
  text-align: center;
  padding: 30px 10px;
  line-height: 30px;
}
</style>