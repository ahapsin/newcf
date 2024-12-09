<template>
    <div class="w-full z-50 flex transparent justify-between p-2">
        <div class="flex z-50 w-full justify-between items-center">
            <div class="flex ">
                <Navbar class="block md:hidden absolute w-1/2 md:w-full" />
                <Logo class="ps-12 md:ps-4" />
            </div>
            <div class="flex items-center gap-2">
                <Navbar class="hidden md:block w-1/2 right-8 md:w-full" />
                <Button asChild size="small">

                    <a href="http://8a73085df21a.sn.mynetname.net:82/bprcf/Auth" target="_blank"><button class="">
                            <div class="flex items-center gap-2 md:border p-2 rounded-full text-primary md:bg-primary/10">
                                <Icon name="ic:baseline-account-circle" size="1.5em" />
                                <span class="flex text-xs md:text:lg">Login</span>
                            </div>
                        </button>
                    </a>
                </Button>
            </div>
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
