<template>
  <div class="container">
    <div class="container-links">
      <p>生徒一覧</p>
      <NuxtLink to="/management">生徒情報を見る</NuxtLink>
    </div>
     <div class="container-links">
      <p>管理者</p>
      <NuxtLink to="/students">管理者画面を見る</NuxtLink>
    </div>
  </div>
</template>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.container-links{
  margin-right:30px;
}
</style>