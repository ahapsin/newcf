<template>
    <div class="card">
        <Menubar :model="items" style="border: 0; background-color: transparent;" class="font-medium">
            <template #item="{ item, props, hasSubmenu }">
                <a :href="item.path" class="flex items-center" v-bind="props.action" v-if="!hasSubmenu">
                    <span>{{ item.label }}</span>
                </a>
                <a v-else class="flex items-center" v-bind="props.action">
                    <span>{{ item.label }}{{ hasSubmenu.path }}</span>
                </a>
            </template>
        </Menubar>
    </div>
</template>

<script setup>
import { ref } from "vue";

const items = ref([
    {
        label: 'Beranda',
        icon: 'pi pi-home',
        path: '/',
    },
    {
        label: 'Produk',
        icon: 'pi pi-search',
        path: '',
        items: [
            {
                label: 'Tabungan',
                icon: 'pi pi-bolt',
                path: '/tabungan',
            },
            {
                label: 'Deposito',
                icon: 'pi pi-server',
                path: '/deposito',
            },
            {
                label: 'Kredit',
                icon: 'pi pi-palette',
                path: '/kredit',
                items: [
                    {
                        label: 'KAMU',
                        icon: 'pi pi-palette',
                        path: '/kredit#kamu',
                    },
                    {
                        label: 'KAMA',
                        icon: 'pi pi-palette',
                        path: '/kredit#kama',
                    },
                    {
                        label: 'KPM',
                        icon: 'pi pi-palette',
                        path: '/kredit#kpm',
                    }
                ]
            }
        ]
    },
    {
        label: 'Tentang Kami',
        icon: 'pi pi-envelope',
        path: '/#visimisi',
        items: [
            {
                label: 'Visi Misi',
                icon: 'pi pi-bolt',
                path: '/#visimisi',
            },
            {
                label: 'Pengumuman',
                icon: 'pi pi-bolt',
                path: '/#pengumuman',
            },
            {
                label: 'Laporan Tahunan',
                icon: 'pi pi-server',
                path: '/#publikasi',
                items: [
                    {
                        label: '2024',
                        path: '/tahunan/2024',
                    },
                ]
            },
            {
                label: 'Laporan Publikasi',
                icon: 'pi pi-server',
                path: '/#publikasi',
                items: [
                    {
                        label: '2024',
                        path: '/publikasi/2024',
                    },
                ]
            },
            {
                label: 'Laporan Tata Kelola',
                icon: 'pi pi-server',
                path: '/#tatakelola',
                items: [
                    {
                        label: '2024',
                        path: '/tata_kelola/2024',
                    },
                ]
            },
            {
                label: 'Laporan Keberlanjutan',
                icon: 'pi pi-server',
                path: '/#publikasi',
                items: [
                    {
                        label: '2024',
                        path: '/keberlanjutan/2024',
                    },
                ]
            },
        ]
    },
    {
        label: 'Kontak Kami',
        icon: 'pi pi-envelope',
        path: '/#contact',
        items: [
            {
                label: 'Layanan Perbankan',
                icon: 'pi pi-bolt',
                path: '/#contact',
            },
            {
                label: 'Pengaduan Nasabah',
                icon: 'pi pi-bolt',
                path: '/pengaduan-nasabah',
            },
            {
                label: 'Whistle blowing System (WBS)',
                icon: 'pi pi-server',
                path: '/wbs',
            }]
    }
]);
</script>
