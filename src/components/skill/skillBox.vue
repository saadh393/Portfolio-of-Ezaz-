<template>
  <div class="skill-title">Skills</div>
  <div class="skill-box">
    <skills imgTitle="Vue js" id="skills">
      1
      <img src="./vue.svg" alt="" />
    </skills>

    <skills imgTitle="Vue js" id="skills">
      2
      <img src="./vue.svg" alt="" />
    </skills>

    <skills imgTitle="Vue js" id="skills">
      3
      <img src="./vue.svg" alt="" />
    </skills>

    <skills imgTitle="Vue js" id="skills">
      4
      <img src="./vue.svg" alt="" />
    </skills>
  </div>
</template>

<script>
import skills from "./skills.vue";

export default {
  name: "skillBox",
  components: {
    skills,
  },
};
</script>

<style lang="scss" scoped>
.skill-title {
  height: 70px;
  width: 500px;
  background: #85848f;
  border-radius: 10px;
  box-shadow: 3px 3px 9px #54535a, -3px -3px 11px #b6b5c4;
  box-sizing: border-box;
  margin: 30px auto;
  margin-bottom: 4rem;
  color: #f4f2db;
  font-family: "Manrope", sans-serif;
  font-size: 40px;
  letter-spacing: 5px;
  text-align: center;
}
.skill-box {
  width: 70%;
  min-height: 350px;
  margin: 20px auto;
  background: #85848f;
  border-radius: 10px;
  box-shadow: 3px 3px 9px #54535a, -3px -3px 11px #b6b5c4;
  box-sizing: border-box;
  padding: 20px;
  box-sizing: border-box;
  display: flex;
  gap: 20px;
  padding: 0 20px;
  box-sizing: border-box;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;

  //display: grid;
  //grid-template-columns: repeat(4, 1fr);
  //grid-template-rows: repeat(2, 1fr);
  // grid-template-columns: repeat(4,1fr);
  // grid-template-rows: repeat(2, 1fr);

  @media screen and (max-width: 1296px) {
    #skills {
      height: 220px;
      width: 180px;
      margin: 1rem auto;
    }
  }
}
</style>
