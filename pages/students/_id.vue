<template>
  <div class="student_id">
    <h2>{{this.students[this.$route.params.id].name}}</h2>
    <div class="link">
    <NuxtLink to="/">トップページ</NuxtLink><span class="text-width">|</span>
    <NuxtLink to="/students">生徒一覧へ戻る</NuxtLink>
    </div>
  </div>
</template>


<script>
export default {
  validate({ params }) {
    if ((params.id === undefined)) {
      return false
    } else {
      return true
    }
  },
  data() {
    return {
      students: [
        {
          id: "qnfungqxllc3m1ak",
          name: "生徒A",
        },
        {
          id: "7j9cumkgsq6l264c",
          name: "生徒B",
        },
        {
          id: "eo34bhey9m0d92ou",
          name: "生徒C",
        },
      ],
    };
  }
};
</script>


<style>
.student_id {
  margin: 10vw auto;
  min-height: 100vh;
  /*display: flex;*/
  /*justify-content: center;
  align-items: center;*/
  text-align: center;
}
.link{
  display: flex;
  justify-content: center;
  margin-top: 20px;
}
.text-width{
  margin: 0 20px;
}
</style>