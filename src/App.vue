<template>
  <main class="container">
    <QrImage />

    <CardTitle :titleMessage="sentences[0].name" />

    <CardPara :paraMessage="sentences[1].name" />
  </main>
  <footer>
    <div class="attribution">
      Challenge by
      <a href="https://www.frontendmentor.io?ref=challenge" target="_blank"
        >Frontend Mentor</a
      >. Coded by <a :href="web">{{ fullName.name }} {{ fullName.lastname }}</a
      >.
    </div>
  </footer>
</template>

<script>
import QrImage from "./components/QrImage.vue";
import CardTitle from "./components/CardTitle.vue";
import CardPara from "./components/CardPara.vue";

export default {
  name: "App",
  components: {
    QrImage,
    CardTitle,
    CardPara,
  },
  data() {
    return {
      sentences: [
        {
          id: 1,
          name: "Improve your front-end skills by building projects",
        },
        {
          id: 2,
          name: "Scan the QR code to visit Frontend Mentor and take your coding skills to the next level",
        },
      ],
      fullName: {
        name: "Arnas",
        lastname: "Luksas",
      },
      web: "https://www.arnasluksas.lt",
    };
  },
};
</script>

<style>

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  background: hsl(212, 45%, 89%);
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
    position: relative;
  min-height: 100vh;

}
.container {
  border-radius: 20px;
  padding: 20px;
  background: white;
  max-width: 375px;

  
}
div {
  font-family: "Outfit", sans-serif;
}
footer {
  text-align: center;
  width: 100%;
  font-size: 15px;
  padding: 5px;
  position: absolute;
  bottom: 0;

}
</style>
