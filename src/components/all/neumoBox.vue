<template>
  <div class="neumo-box">
    <h1><slot name="HeadText"></slot></h1>
    <p><slot name="ParagraphText"></slot></p>
  </div>
</template>

<script>
export default {
  name: "neumo-box",
};
</script>

<style lang="scss">
.neumo-box {
  height: 270px;
  max-width: 550px;
  background: #85848f;
  border-radius: 10px;
  box-shadow: 5px 5px 10px #54535a, -5px -5px 22px #b6b5c4;
  box-sizing: border-box;

  @media screen and (max-width: 600px) {
    width: 80%;
  }

  h1,
  p {
    color: #f4f2db;
    padding-left: 40px;
    position: relative;
    font-family: "Manrope", sans-serif;
  }
  h1 {
    top: 45px;
    font-size: 40px;
  }
  p {
    top: 65px;
    font-size: 18px;
  }
}
</style>
