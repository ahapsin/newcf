<template>
  <div class="flex bg-slate-50 w-screen h-screen justify-center overflow-auto">
    <div class="bg-slate-50 w-[1366px]">
      <LandingHeader/>
      <div class="p-4">
        <slot />
      </div>
      <LandingFooter/>
    </div>
  </div>
</template>

<script lang="ts" setup>

</script>

<style scoped>
@keyframes slidedown-icon {
  0% {
      transform: translateY(0);
  }

  50% {
      transform: translateY(20px);
  }

  100% {
      transform: translateY(0);
  }
}

.slidedown-icon {
  animation: slidedown-icon;
  animation-duration: 3s;
  animation-iteration-count: infinite;
}
</style>
