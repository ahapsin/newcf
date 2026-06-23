<template>
    <div class="card mt-14 max-w-[1366px] mx-auto">
        <Tabs value="0" scrollable>
            <TabList>

                <Tab value="0">
                    <Badge value="1" severity="warn"></Badge> Struktur Organisasi Pelindungan Konsumen
                </Tab>
                <Tab value="1">
                    <Badge value="2" severity="warn"></Badge> Mekanisme Penanganan
                </Tab>
                <Tab value="2">
                    <Badge value="3" severity="warn"></Badge> Layanan Nasabah APPK
                </Tab>
                <Tab value="3">
                    <Badge value="4" severity="warn"></Badge> Form Pengaduan
                </Tab>
            </TabList>
            <TabPanels>
                <TabPanel value="0">
                    <SectionProsedur />
                </TabPanel>
                <TabPanel value="1">
                    <h2 class=" md:text-2xl mb-4">1. Pengaduan Secara Lisan</h2>
                    <div class="flex justify-center w-full bg-red-500">
                        <img src="/pengaduan/Alur_Pengaduan_Lisan.webp" class="w-full h-full object-cover" alt="" />
                    </div>
                    <h2 class="md:text-2xl my-4">2. Pengaduan Secara Tertulis</h2>
                    <div class="flex justify-center w-full mx-auto">
                        <img src="/pengaduan/Alur_Pengaduan_Tertulis.webp" class="w-full h-full object-cover" alt="" />
                    </div>
                    <h2 class="md:text-2xl my-4">3. Alur Layanan Pengaduan Nasabah</h2>
                    <div class="flex justify-center w-full mx-auto">
                        <img src="/pengaduan/Alur_Layanan_Pengaduan_Nasabah.webp" class="w-full h-full object-cover"
                            alt="" />
                    </div>
                </TabPanel>
                <TabPanel value="2">
                    <div class="flex justify-center">
                        <img src="/public/layanan_pengaduan.jpg" />
                    </div>

                    <div class="flex justify-center">

                        <div class="md:w-3/4">
                            <h2>Keterangan</h2>
                            1. Nasabah membuka Website APPK dengan memasukkan alamat link
                            yaitu
                            <b>www.kontak157.ojk.go.id</b><br />
                            2. Setelah terhubung pada layanan APPK, kemudian - Pilih menu Ticketing – Pilih menu
                            Form Pengaduan Online, atau dapat juga klik PENGADUAN (contoh : gambar di
                            atas).<br />
                            3. Nasabah dapat melakukan pengisian pengajuan pengaduan yang terdiri dari 5 tahapan
                            yaitu:<br />
                            - Pilih permasalahan dan PUJK - Isi Kronologis Kejadian - Isi Data Diri - Unggah
                            Lampiran - Kemudian Klik Kirim Pengaduan.<br />
                            4. Nomor Layanan dan Pin/Tiket Layanan Pengaduan Nasabah akan muncul dan dikirimkan
                            melalui alamat<b> Email</b> yang didaftarkan jika Nasabah lupa Nomor tersebut.<br />
                            5. Nasabah wajib menyiapkan lampiran-lampiran yang dibutuhkan dalam hal Pengaduan
                            sesuai
                            dengan yang diminta dalam APPK.<br />
                            6. Setelah Pengaduan Nasabah ditindaklanjuti oleh Bank, maka Nasabah dapat melakukan
                            pengecekan pada Website APPK dan Pilih menu Ticketing – Pilih Menu cek Status
                            Pengaduan
                            dengan mengisi Nomor Layanan dan Pin/Tiket yang telah diperoleh pada saat melakukan
                            Pengaduan.<br />
                            7. Apabila ada dokumen tambahan yang wajib dipenuhi oleh Nasabah, maka Nasabah dapat
                            langsung menambahkan dokumen tersebut pada saat cek status pengaduan tersebut –
                            kemudian
                            Simpan Dokumen Tambahan – Klik OK.<br />
                            8. Dalam hal Nasabah menolak solusi yang diberikan oleh Bank atau Nasabah merasa
                            tidak
                            puas terhadap jawaban Pengaduan, maka Nasabah dapat klik tombol Tolak Solusi PUJK –
                            Pilh
                            dilanjutkan ke LAPS atau tidak.
                        </div>
                    </div>
                </TabPanel>
                <TabPanel value="3">
                    <SectionPengaduan />
                </TabPanel>
            </TabPanels>
        </Tabs>
    </div>
</template>

<script lang="ts" setup>

definePageMeta({
    layout: 'landing'
})
</script>
