<template>
  <div id="app">
    <h1>JavaScript calculator</h1>
    <div id="drum-machine">
      <div id="display">
        <AppDrumPad msg="1" id="one"></AppDrumPad>
        <AppDrumPad msg="2" id="two"></AppDrumPad>
        <AppDrumPad msg="3" id="three"></AppDrumPad>
        <AppDrumPad msg="+" id="add"></AppDrumPad>
        <AppDrumPad msg="4" id="four"></AppDrumPad>
        <AppDrumPad msg="5" id="five"></AppDrumPad>
        <AppDrumPad msg="6" id="six"></AppDrumPad>
        <AppDrumPad msg="-" id="subtract"></AppDrumPad>
        <AppDrumPad msg="7" id="seven"></AppDrumPad>
        <AppDrumPad msg="8" id="eight"></AppDrumPad>
        <AppDrumPad msg="9" id="nine"></AppDrumPad>
        <AppDrumPad msg="*" id="multiply"></AppDrumPad>
        <AppDrumPad msg="=" id="equals"></AppDrumPad>
        <AppDrumPad msg="0" id="zero"></AppDrumPad>
        <AppDrumPad msg="." id="decimal"></AppDrumPad>
        <AppDrumPad msg="/" id="divide"></AppDrumPad>
        <AppDrumPad msg="Clear" id="clear"></AppDrumPad>
      </div>
    </div>
  </div>
</template>

<script>
import AppDrumPad from "./components/AppDrumPad.vue";

export default {
  name: "app",
  components: {
    AppDrumPad
  },
  mounted() {
    let recaptchaScript = document.createElement("script");
    recaptchaScript.setAttribute(
      "src",
      "https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js"
    );
    document.head.appendChild(recaptchaScript);
  }
};
</script>

<style>
@import url("https://fonts.googleapis.com/css?family=Bubbler+One&display=swap");

* {
  margin: 0;
  padding: 0;
  background-color: #262621;
}

#app {
  font-family: "Bubbler One", sans-serif;
  font-weight: 100;
  text-align: center;
}
#drum-machine {
  width: 80%;
  margin: 0 auto;
}

#display {
  display: grid;
  grid-template-columns: 125px 125px 125px 125px;
  grid-template-rows: 125px 125px 125px 125px 125px;
  grid-column-gap: 15px;
  grid-row-gap: 15px;
  justify-content: center;
  background-color: #5679a6;
  border-radius: 25px;
  padding: 15px;
}

h1 {
  font-size: 50px;
  margin: 25px;
  color: #fff;
}

#clear {
  width: 560px;
}
</style>
