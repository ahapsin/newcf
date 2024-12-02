<template>
  <div class="flex justify-between p-4">
    <div class="flex items-center gap-x-32">
      <Logo/>
    </div>
    <div class="flex">
      <Navbar/>
      <Button asChild size="small">
        <button class="">
          <div class="flex items-center gap-2 border p-2 rounded-full text-primary bg-primary/10">
            <Icon name="ic:baseline-account-circle" size="1.5em" />
            Login
          </div>
        </button>
      </Button>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const items = ref([
  {
    label: 'Home',
    icon: 'pi pi-home'
  },
  {
    label: 'Projects',
    icon: 'pi pi-search',
    badge: 3,
    items: [
      {
        label: 'Core',
        icon: 'pi pi-bolt',
        shortcut: '⌘+S'
      },
      {
        label: 'Blocks',
        icon: 'pi pi-server',
        shortcut: '⌘+B'
      },
      {
        separator: true
      },
      {
        label: 'UI Kit',
        icon: 'pi pi-pencil',
        shortcut: '⌘+U'
      }
    ]
  }
]);
</script>
