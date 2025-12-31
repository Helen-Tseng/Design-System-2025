<template>
  <div class="l-divider">
  <p>橫式</p>
    <hr class="l-divider-horizontal border-gray05">
    <hr class="l-divider-horizontal border-primary03">
    <p>直式</p>
    <hr class="l-divider-straight border-gray05">
    <hr class="l-divider-straight border-primary03">
  </div>
</template>

<style scoped>
.l-divider{
  position: relative;
  display: inline-block;
  width: 50%;
}
.l-divider-horizontal { 
  border-top: 1px solid;
  width: 100%;
  margin: 40px 0;
  }
  .l-divider-straight{
    display: inline-block;
    margin: 0 30px;
      border-top: none;
      border-left: 1px solid;
      height: 200px;
  }
  .border-gray05{
    border-color: #d9d9d9;
  }
  .border-primary03{
    border-color: #bde3e2;
  }

</style>