<template>
    <div class="max-w-5xl mx-auto p-6 bg-white rounded-lg  space-y-6">
        <!-- Header -->
        <section class="text-center">
            <h1 class="text-2xl font-bold text-primary">Produk Tabungan Cahaya Fajar</h1>
            <p class="text-lg text-gray-600">PT. BPR CAHAYA FAJAR</p>
        </section>

        <!-- Informasi Umum -->
        <section>
            <h2 class="text-xl font-semibold text-primary mb-2">Informasi Umum</h2>
            <ul class="list-disc list-inside text-gray-700 space-y-1">
                <li>Jenis Produk: Tabungan</li>
                <li>Produk simpanan perorangan yang penyetorannya dapat dilakukan setiap saat.</li>
                <li>Tidak dibatasi jangka waktu dan frekuensi penarikan sepanjang saldo mencukupi.</li>
            </ul>
        </section>

        <!-- Fitur Utama -->
        <section>
            <h2 class="text-xl font-semibold text-primary mb-2">Fitur Utama</h2>
            <div class="grid grid-cols-2 gap-4 text-gray-700">
                <div>Simpanan Awal: <strong>Rp. 100.000,-</strong></div>
                <div>Saldo Minimal: <strong>Rp. 100.000,-</strong></div>
                <div>Setoran Selanjutnya: <strong>Tidak ada batasan</strong></div>
                <div>Minimal Penarikan Tunai: <strong>Rp. 100.000,-</strong></div>
            </div>
            <div class="mt-4">
                <h3 class="font-medium text-gray-800">Bunga Tabungan:</h3>
                <table class="w-full mt-2 table-auto border border-gray-300 text-sm">
                    <thead class="bg-gray-100">
                        <tr>
                            <th class="border px-2 py-1">Nominal</th>
                            <th class="border px-2 py-1">Suku Bunga p.a</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td class="border px-2 py-1">≤ Rp. 100.000.000,-</td>
                            <td class="border px-2 py-1">0.5%</td>
                        </tr>
                        <tr>
                            <td class="border px-2 py-1">&gt; Rp. 100.000.000,- s/d Rp. 2.000.000.000,-</td>
                            <td class="border px-2 py-1">1%</td>
                        </tr>
                        <tr>
                            <td class="border px-2 py-1">&gt; Rp. 2.000.000.000,- s/d Rp. 4.000.000.000,-</td>
                            <td class="border px-2 py-1">2%</td>
                        </tr>
                        <tr>
                            <td class="border px-2 py-1">&gt; Rp. 4.000.000.000,- s/d Rp. 5.000.000.000,-</td>
                            <td class="border px-2 py-1">3%</td>
                        </tr>
                        <tr>
                            <td class="border px-2 py-1">&gt; Rp. 5.000.000.000,-</td>
                            <td class="border px-2 py-1">4%</td>
                        </tr>
                    </tbody>
                </table>
            </div>
            <p class="mt-2 text-sm text-gray-600 italic">Tingkat Bunga Penjaminan LPS: <strong>6,25%</strong></p>
        </section>

        <!-- Biaya -->
        <section>
            <h2 class="text-xl font-semibold text-primary mb-2">Biaya</h2>
            <ul class="list-disc list-inside text-gray-700 space-y-1">
                <li>Biaya Administrasi: Tidak ada</li>
                <li>Biaya Penutupan Rekening: Rp. 5.000,-</li>
                <li>Biaya Administrasi Rekening Pasif: Rp. 1.000,- / bulan</li>
            </ul>
        </section>

        <!-- Manfaat dan Risiko -->
        <section>
            <h2 class="text-xl font-semibold text-primary mb-2">Manfaat dan Risiko</h2>
            <ul class="list-disc list-inside text-gray-700 space-y-1">
                <li>Suku bunga menarik dan tinggi.</li>
                <li>Mudah dalam pembukaan rekening dan pelayanan cepat.</li>
                <li>Penarikan dapat dilakukan dengan setor tunai, transfer antar bank, dan pemindahbukuan.</li>
                <li>Risiko perubahan suku bunga tabungan.</li>
                <li>Tidak dijamin LPS jika: bunga lebih tinggi dari penjaminan LPS, nominal simpanan melebihi yang
                    dijamin LPS, atau bank tidak ikut serta dalam penjaminan LPS.</li>
            </ul>
        </section>

        <!-- Syarat & Kontak -->
        <section>
            <h2 class="text-xl font-semibold text-primary mb-2">Persyaratan dan Tata Cara</h2>
            <ul class="list-disc list-inside text-gray-700 space-y-1">
                <li>Membawa KTP/SIM/Paspor sesuai ketentuan.</li>
                <li>Mengisi formulir pembukaan rekening.</li>
                <li>Menandatangani dokumen lainnya sesuai ketentuan bank.</li>
            </ul>

            <h3 class="font-medium text-gray-800 mt-4">Informasi Lebih Lanjut:</h3>
            <ul class="text-gray-700">
                <li>Telp: (021) 2480490 / 2480620 / 248922</li>
                <li>Email: <a href="mailto:bprcahayafajar@yahoo.co.id"
                        class="text-primary underline">bprcahayafajar@yahoo.co.id</a></li>
                <li>Website: <a href="http://www.bprcahayafajar.co.id" target="_blank"
                        class="text-primary underline">www.bprcahayafajar.co.id</a></li>
            </ul>
        </section>
    </div>
</template>

<script setup>
// No logic needed for static info
</script>

<style scoped>
/* Optional: custom styles if needed */
</style>
