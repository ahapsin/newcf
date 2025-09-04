<template>
    <div>
        <Title name="title">Tabungan BPR Cahaya Fajar</Title>
        <div>
        </div>
        <div class="p-20">
            <Fieldset>
                <template #legend>
                    <div class="flex items-center pl-2">
                        <span class="font-bold p-2">Deposito Personal</span>
                    </div>
                </template>
                <div class="pdf-container">
                    <iframe src="/product/DEPOSITO/RIPLAY PERSONAL Deposito Cahaya Fajar.pdf" width="100%" height="600px"
                        style="border: none;"></iframe>
                </div>
            </Fieldset>
            <Fieldset>
                <template #legend>
                    <div class="flex items-center pl-2">
                        <span class="font-bold p-2">Deposito Umum</span>
                    </div>
                </template>
 <div class="pdf-container">
                    <iframe src="/product/DEPOSITO/RIPLAY UMUM Deposito Cahaya Fajar.pdf" width="100%" height="600px"
                        style="border: none;"></iframe>
                </div>
            </Fieldset>

        </div>
    </div>
</template>

<script lang="ts" setup>

definePageMeta({
    layout: 'landing'
})
</script>
