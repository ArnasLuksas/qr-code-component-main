<template>
  <div>
    <img :src="image" alt="" />
  </div>
</template>

<script>
export default {
  name: "QrImage",
  data() {
    return {
      image: require("../assets/image-qr-code.png"),
    };
  },
};
</script>


<style scoped>
img {
  width: 100%;
  height: 100%;
  border-radius: 20px;
}
</style>