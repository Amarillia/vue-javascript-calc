<template>
  <div class="drum-pad">
    <button>{{msg}}
    </button>
  </div>
</template>

<script>
export default {
  name: "AppDrumPad",
  props: {
    msg: String,
   }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.drum-pad {
background:none;
}

button {
  border: 1px solid #A6123A;
  background-color: #A6123A;
  font-size: 55px;
  width: 125px;
  height: 125px;
  cursor: pointer;
  border-radius: 25px;
  color: #BFBDB0;
}
</style>
