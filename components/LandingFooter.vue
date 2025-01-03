<template>
    <div class="flex gap-10 bg-surface-200 dark:bg-primary-700 p-10 px-14 justify-between">
        <div class="flex flex-col items-start gap-x-32">
            <div class="w-[180px] py-4">
                <Logo />
            </div>
            <div class="flex flex-col bg-surface-200 dark:bg-primary-700 text-muted-color text-xs ">
                PT. Bank Perekonomian Rakyat Cahaya Fajar terdaftar dan diawasi oleh: <br />
                <strong>Otoritas Jasa Keuangan (OJK) & Lembaga Penjamin Simpanan (LPS)</strong><br />
                <small>&copy; BPRcahayafajar 2024. All rights reserved.</small>
            </div>
        </div>
        <div class="flex gap-10" v-if="false">
            <Card unstyled class="text-surface-800">
                <template #title><strong>Simple Card</strong></template>
                <template #content>
                    <div class="flex flex-col">
                        <NuxtLink to="/about">
                            About page
                        </NuxtLink>
                        <NuxtLink to="/about">
                            About page
                        </NuxtLink>
                        <NuxtLink to="/about">
                            About page
                        </NuxtLink>
                    </div>
                </template>
            </Card>
            <Card unstyled class="text-surface-800">
                <template #title><strong>Simple Card</strong></template>
                <template #content>
                    <div class="flex flex-col">
                        <NuxtLink to="/about">
                            About page
                        </NuxtLink>
                        <NuxtLink to="/about">
                            About page
                        </NuxtLink>
                        <NuxtLink to="/about">
                            About page
                        </NuxtLink>
                    </div>
                </template>
            </Card>
            <Card unstyled class="text-surface-800">
                <template #title><strong>Simple Card</strong></template>
                <template #content>
                    <div class="flex flex-col">
                        <NuxtLink to="/about">
                            About page
                        </NuxtLink>
                        <NuxtLink to="/about">
                            About page
                        </NuxtLink>
                        <NuxtLink to="/about">
                            About page
                        </NuxtLink>
                    </div>
                </template>
            </Card>
        </div>
        <div class="flex flex-col gap-y-4">
            <span>folow us on</span>
            <div class="flex gap-2">
              <NuxtLink to="https://www.youtube.com/@bprcahayafajar8816">
                <Button size="small" severity="secondary" unstyled>
                    <Icon name="line-md:youtube" size="1.5em" class="text-primary" />
                </Button>
              </NuxtLink>
              <NuxtLink to="https://www.instagram.com/bprcahayafajar_/">
                <Button size="small" severity="secondary" unstyled>
                    <Icon name="line-md:instagram" size="1.3em" class="text-primary" />
                </Button>
              </NuxtLink>
              <NuxtLink to="https://www.instagram.com/bprcahayafajar_/">
                <Button size="small" severity="secondary" unstyled>
                    <Icon name="line-md:twitter-x" size="1.2em" class="text-primary" />
                </Button>
              </NuxtLink>
            </div>
        </div>
    </div>

</template>

<script lang="ts" setup>

</script>

<style>

</style>
