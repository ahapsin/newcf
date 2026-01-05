<template>
    <div class="flex">
        <div class="flex w-full items-center justify-center">
            <img src="/public/wbs.jpg" />
        </div>
        <div class="w-full p-10">
            <div class="text-2xl font-bold pb-8">WBS - Whistle Blower System</div>
            <div class="flex flex-col gap-4">
                <div class="flex flex-col gap-2">
                    <label for="username">Nama Pelapor</label>
                    <InputText id="username" v-model="formData.nama_pelapor" aria-describedby="username-help"
                        placeholder="Nama Anda" />
                </div>
                <div class="flex flex-col gap-2">
                    <label for="username">Nomor Telepon</label>
                    <InputText id="username" v-model="formData.no_telpon" aria-describedby="username-help"
                        placeholder="Nomor Telepon  / whatsapp yang bisa dihubungi" />
                </div>
                <div class="flex flex-col gap-2">
                    <label for="username">Tanggal Kejadian</label>
                    <DatePicker v-model="formData.tgl_kejadian" placeholder="tanggal kejadian"
                        v-model:value="formData.tgl_kejadian" />
                </div>
                <div class="flex flex-col gap-2">
                    <label for="username">Jenis aduan</label>
                    <Select v-model="formData.jenis_aduan" :options="jenis" optionLabel="name"
                        placeholder="pilih jenis aduan" class="w-full md:w-56" />
                </div>
                <div class="flex flex-col gap-2">
                    <label for="username">Penjelasan / Keterangan</label>
                    <Textarea v-model="formData.keterangan" rows="5" cols="30" />
                </div>
                <div class="flex flex-col gap-2 justify-start">
                    <label for="username">Bukti</label>
                    <FileUpload ref="fileupload" mode="basic" name="demo[]" url="/api/upload" accept="image/*"
                        :maxFileSize="1000000" @upload="onUpload" />
                </div>
                <div class="flex flex-col gap-2">
                    <Button @click="handleSubmit">Kirim</Button>
                </div>
            </div>
        </div>
    </div>
    <Dialog v-model:visible="visible" modal @after-hide="onClose" header="Terima kasih" :style="{ width: '50rem' }"
        :breakpoints="{ '1199px': '75vw', '575px': '90vw' }">
        <p class="m-0">
            Laporan Anda telah kami terima dan akan ditindaklanjuti sesuai prosedur yang berlaku. Kerahasiaan identitas
            Anda kami jaga sepenuhnya.
        </p>
    </Dialog>
    <Button label="Show" @click="visible = true" />
</template>

<script setup>

const visible = ref(false);
const loading = ref(false)
const success = ref(false)
const errorMsg = ref(null)

const handleSubmit = async () => {
    loading.value = true
    success.value = false
    errorMsg.value = null

    try {
        const res = await $fetch('https://api.bprcahayafajar.co.id/email_send', {
            method: 'POST',
            body: formData.value
        })

        // on finish SUCCESS
        success.value = true
        visible.value = true;

    } catch (error) {
        // on finish ERROR
        errorMsg.value = 'Gagal mengirim laporan'
    } finally {
        // selalu dipanggil saat selesai
        loading.value = false
    }
}
const formData = ref({
    nama_pelapor: null,
    no_telpon: null,
    tgl_kejadian: null,
    jenis_aduan: null,
    keterangan: null,
});

const jenis = ref([
    { name: 'Permasalahan terkait produk tabungan' },
    { name: 'Permasalahan terkait produk deposito' },
    { name: 'Permasalahan terkait produk kredit' },
    { name: 'Permasalahan Lainnya' },
]);
const onClose = () => {
    formData.value = {
        nama_pelapor: null,
        no_telpon: null,
        tgl_kejadian: null,
        jenis_aduan: null,
        keterangan: null,
    }
}
</script>
