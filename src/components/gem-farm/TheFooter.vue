<template>
  <div class="footer bg-footer pt-1 pb-1">
    <p class="px-3 text-aqua-1">Copy with</p>
    <i class="nes-icon heart"></i>
    <p class="text-aqua-1 px-3">
      by
      <a
        class="nes-text text-black"
        href="https://twitter.com/_ilmoi"
        target="_blank"
        >@gynchiii</a
      >
      | powered by
      <a
        class="nes-text text-black"
        href="https://twitter.com/GenesysGo"
        target="_blank"
        >GenesysGo</a
      >
    </p>
    <img src="../../assets/gg_logo.png" height="31" width="28" />
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.text-aqua-1 {
  color: rgb(188, 219, 210);
}
.bg-footer{
  background-color: rgb(56, 105, 90);
}
.footer {
  @apply w-full flex justify-center align-middle text-center;
  position: absolute;
  bottom: 0px;
  height: 40px;
}
</style>
