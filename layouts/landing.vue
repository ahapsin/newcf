<template>
    <div ref="el" class="relative bg-white w-screen h-screen justify-center overflow-auto">
        <div class="w-full">
            <div class="fixed top-0 pe-4 w-full z-50" :class="!arrivedState.top ? 'bg-white shadow-xl' :'bg-transparent '">
                <LandingHeader />
            </div>
            <div>
                <slot />

            </div>
            <LandingFooter />

        </div>
    </div>
</template>

<script lang="ts" setup>
const el = ref<HTMLElement | null>(null)
const { x, y, isScrolling, arrivedState, directions } = useScroll(el)
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
