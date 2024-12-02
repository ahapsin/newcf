<template>
  <div class="card">
    <Menubar :model="items" style="border: 0; background-color: transparent;"/>
  </div>
</template>

<script setup>
import { ref } from "vue";

const items = ref([
  {
    label: 'Beranda',
    icon: 'pi pi-home'
  },
  {
    label: 'Produk',
    icon: 'pi pi-search',
    items: [
      {
        label: 'Components',
        icon: 'pi pi-bolt'
      },
      {
        label: 'Blocks',
        icon: 'pi pi-server'
      },
      {
        label: 'UI Kit',
        icon: 'pi pi-pencil'
      },
      {
        label: 'Templates',
        icon: 'pi pi-palette',
        items: [
          {
            label: 'Apollo',
            icon: 'pi pi-palette'
          },
          {
            label: 'Ultima',
            icon: 'pi pi-palette'
          }
        ]
      }
    ]
  },
  {
    label: 'Tentang Kami',
    icon: 'pi pi-envelope'
  },
  {
    label: 'Kontak',
    icon: 'pi pi-envelope'
  }
]);
</script>
