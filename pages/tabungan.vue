<template>
    <div>
        <Title name="title">Tabungan BPR Cahaya Fajar</Title>
        <div>
        </div>
        <div class="p-20">
            <Fieldset>
                <template #legend>
                    <div class="flex items-center pl-2">
                        <span class="font-bold p-2">Tabungan Personal</span>
                    </div>
                </template>
                <Tabs value="0">
                    <TabList>
                        <Tab value="0">Cahaya Fajar</Tab>
                        <Tab value="1">Ciremaiku</Tab>
                        <Tab value="2">TabunganKu</Tab>
                    </TabList>
                    <TabPanels>
                        <TabPanel value="0">
                            <div class="pdf-container">
                                <iframe src="/product/TABUNGAN/PERSONAL/RIPLAY PERSONAL Tabungan Cahaya Fajar.pdf" width="100%"
                                    height="600px" style="border: none;"></iframe>
                            </div>
                        </TabPanel>
                        <TabPanel value="1">
                            <div class="pdf-container">
                                <iframe src="/product/TABUNGAN/PERSONAL/RIPLAY PERSONAL Tabungan Ciremaiku.pdf" width="100%"
                                    height="600px" style="border: none;"></iframe>
                            </div>
                        </TabPanel>
                        <TabPanel value="2">
                            <div class="pdf-container">
                                <iframe src="/product/TABUNGAN/PERSONAL/RIPLAY PERSONAL TabunganKu.pdf" width="100%"
                                    height="600px" style="border: none;"></iframe>
                            </div>
                        </TabPanel>
                    </TabPanels>
                </Tabs>
            </Fieldset>
            <Fieldset>
                <template #legend>
                    <div class="flex items-center pl-2">
                        <span class="font-bold p-2">Tabungan Umum</span>
                    </div>
                </template>
                <Tabs value="0">
                    <TabList>
                        <Tab value="0">Cahaya Fajar</Tab>
                        <Tab value="1">Ciremaiku</Tab>
                        <Tab value="2">TabunganKu</Tab>
                    </TabList>
                    <TabPanels>
                        <TabPanel value="0">
                           <div class="pdf-container">
                                <iframe src="/product/TABUNGAN/UMUM/RIPLAY UMUM Tabungan Cahaya Fajar.pdf" width="100%"
                                    height="600px" style="border: none;"></iframe>
                            </div>
                        </TabPanel>
                        <TabPanel value="1">
                           <div class="pdf-container">
                                <iframe src="/product/TABUNGAN/UMUM/RIPLAY UMUM Tabungan Ciremaiku.pdf" width="100%"
                                    height="600px" style="border: none;"></iframe>
                            </div>
                        </TabPanel>
                        <TabPanel value="2">
                            <div class="pdf-container">
                                <iframe src="/product/TABUNGAN/UMUM/RIPLAY UMUM TabunganKu.pdf" width="100%"
                                    height="600px" style="border: none;"></iframe>
                            </div>
                        </TabPanel>
                    </TabPanels>
                </Tabs>
            </Fieldset>

        </div>
    </div>
</template>

<script lang="ts" setup>

definePageMeta({
    layout: 'landing'
})
</script>
