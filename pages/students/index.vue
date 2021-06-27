<template>
  <div class="students">
     <h2>生徒一覧</h2>
     <ul v-for="(student,index) in students" v-bind:key="index">
       <li> <NuxtLink :to="`students/${index}`">{{student.name}}</NuxtLink></li>
    </ul>
      <p class="center"><NuxtLink to="/">戻る</NuxtLink></p>
  </div>
</template>


<script>
export default {
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
  },
};
</script>


<style>
.students {
  margin: 10vw auto;
  /*min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;*/
  width: 8%;
  text-align: center;
}
.students h2{
margin-bottom: 20px;
}
.center{
  margin-top: 10px;
}
</style>