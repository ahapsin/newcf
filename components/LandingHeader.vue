<template>
    <div class="w-full flex transparent justify-center p-2">
        <div class="flex  w-[1366px] justify-between items-center">
            <div class="flex items-center">
                <Navbar class="block md:hidden absolute w-1/2 md:w-full" v-if="props.headLess" />
                <Logo class="ps-12 md:ps-4 w-[180px]" v-if="props.headLess" />
                <LogoMinus class="ps-12 md:ps-4" v-else />
            </div>
            <div class="flex items-center gap-2">
                <Navbar class="hidden md:block w-1/2 right-8 md:w-full" v-if="props.headLess" />
                <Button asChild size="small" v-if="props.headLess">
                    <a href="http://8a73085df21a.sn.mynetname.net:82/bprcf/Auth" target="_blank"><button class="">
                            <div
                                class="flex items-center gap-2 md:border pr-2 rounded-full dark:border-orange-500 text-primary dark:text-white md:bg-primary/10">
                                <Icon name="ic:baseline-account-circle" size="2em" />
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

const props = defineProps({
    headLess: {
        type: Boolean,
        default: true,
    },
});

const isDark = useDark()
const toggleDark = useToggle(isDark)

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
