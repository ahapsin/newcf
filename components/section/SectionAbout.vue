<template>
    <div class="p-4 md:p-20 gap-4 flex flex-col bg-surface-50" id="about">
        <div class="flex flex-col md:flex-row gap-4 mt-10"
            v-animateonscroll="{ enterClass: 'animate-fadein', leaveClass: 'animate-slideout' }">
            <div class="bg-primary-50/10 rounded-xl p-4 w-full animate-duration-1000 animate-ease-in-out"
                v-animateonscroll="{ enterClass: 'animate-fadein', leaveClass: 'animate-slideout' }">
                <div class="text-orange-500">Visi Perusahaan</div>
                <div class="text-xl">Menjadi BPR Terbaik dan Terpercaya bagi Masyarakat Cirebon</div>
            </div>
            <div class="bg-primary-50/10 rounded-xl p-4 w-full">
                <div class="text-orange-500">Misi Perusahaan</div>
                <div class="text-xl first-letter:float-left
    first-letter:text-2xl
    first-letter:text-blue-900 first-letter:font-bold">Memberikan pelayanan perbankan terbaik bagi kepuasan dan
                    loyalitas nasabah. <small class="text-primary" @click="showMisi = !showMisi">lihat semua</small>
                </div>
                <div class="text-xl
    first-letter:text-2xl
    first-letter:text-blue-900 first-letter:font-bold" v-if="showMisi">Mewujudkan tata kelola BPR yang baik untuk
                    meningkatkan
                    produktifitas dan
                    pertumbuhan BPR.</div>
                <div class="text-xl
    first-letter:text-2xl
    first-letter:text-blue-900 first-letter:font-bold" v-if="showMisi">Membentuk sumber daya manusia yang profesional
                    dan berintegritas
                    tinggi</div>
                <div class="text-xl first-letter:text-2xl
    first-letter:text-blue-900 first-letter:font-bold" v-if="showMisi">Mensejahterakan dan memberikan nilai tambah
                    kepada seluruh
                    stakeholders.</div>
                <div class="text-xl first-letter:text-2xl
    first-letter:text-blue-900 first-letter:font-bold" v-if="showMisi">Memberikan manfaat yang baik bagi masyarakat
                    sekitar.</div>
            </div>
            <div class="bg-primary-50/10 rounded-xl p-4 w-full">
                <div class="text-orange-500">Nilai Perusahaan</div>
                <div class="text-xl">Setia, Adaptif, Komitmen, Tangguh ,Inisiatif (<b>S.A.K.T.I</b>)</div>
            </div>

        </div>
        <div class="flex  justify-between items-center bg-primary text-white rounded-xl p-4 w-full">
            <div class="text-xl">Laporan Tata Kelola BPR Cahaya Fajar</div>
            <Button as="a" label="Lihat" severity="warn"
                href="https://api.bprcahayafajar.co.id/storage/File_Upload/n985CtYawKgK990riJz9qJxSKyMtTICctgf6UyHA.pdf"
                target="_blank" rel="noopener" />
        </div>
    </div>
</template>
<script setup>
const showMisi = ref(false);
</script>
