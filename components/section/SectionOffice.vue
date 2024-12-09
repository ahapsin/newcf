<script setup>
const cabang = [
    {
        "nama_kantor": "Kantor Pusat",
        "alamat": "Jl. Karanggetas No. 142, Cirebon",
        "telepon": ["0231-248400", "0231-248600", "0231-248222"],
        "fax": "0231-204520",
        "location":"https://maps.app.goo.gl/4J3d4d7T23jEH7sz8",
    },
    {
        "nama_kantor": "Kantor Cabang Pabuaran",
        "alamat": "Jl. Letjen S Parman, Pabuaran Kidul, Kab. Cirebon",
        "telepon": ["0231-663790", "0231-663789"],
        "fax": "0231-663788",
        "location":"https://maps.app.goo.gl/aCiQ1WYJhJ8Gz89DA",
    },
    {
        "nama_kantor": "Kantor Cabang Jatibarang",
        "alamat": "Jl. Raya Bulak No. 13-14, Jatibarang, Kab. Indramayu",
        "telepon": ["0234-355583", "0234-355585"],
        "fax": "0234-351210",
        "location":"https://maps.app.goo.gl/Up5E9PT6iPgCgCPc6",
    },
    {
        "nama_kantor": "Kantor KAS Plered",
        "alamat": "Jl. Ir. H Juanda No. 22, Plered",
        "telepon": ["0231-321666"],
        "fax": null,

    },
    {
        "nama_kantor": "Kantor Cabang Jatiwangi",
        "alamat": "Komplek Ruko Jatiwangi Square Blok A No. 26, Kabupaten Majalengka",
        "telepon": ["0233-360100", "081222549115"],
        "fax": null,
        "location": "https://maps.app.goo.gl/cHtpVRohwdDpSSp79",
    },
    {
        "nama_kantor": "Kantor Cabang Kuningan",
        "alamat": "Jl. Syeh Maulana Akbar No. 18, Citamba, Kabupaten Kuningan",
        "telepon": ["0232-8951005", "0232-6001041"],
        "fax": null,
        "location": "https://maps.app.goo.gl/C97Ch75v8VBY4q2s7",
    }
]
</script>

<template>
    <div id="contact"
        class="animate-duration-1000 animate-ease-in-out">
        <div class="p-4 text-white px-10 bg-surface-50"></div>
        <div class="flex justify-center  pt-10 text-orange-500 font-semibold  bg-primary text-2xl">
            Kantor Pelayanan Cabang
        </div>
        <div class="grid md:grid-cols-3 p-4 md:p-20 gap-4 bg-primary ">
            <div class="bg-primary-400 p-4 rounded-xl text-white animate-duration-1000 animate-ease-in-out"
                v-for="branch in cabang"
                v-animateonscroll="{ enterClass: 'animate-fadein', leaveClass: 'animate-slideout' }">
                <div class="flex justify-between text-xl font-semibold ">
                    {{ branch.nama_kantor }}
                    <Button as="a" :href="branch.location" severity="secondary" rounded variant="outlined"
                        target="_blank" aria-label="Bookmark" unstyled
                        class="w-10 rounded-full bg-orange-500 text-orange-200 flex items-center justify-center aspect-square">
                        <Icon name="ic:round-location-on" />
                    </Button>
                </div>
                <div>
                    <span class="text-white/50 text-sm">{{ branch.alamat }}
                        <br />
                        <span v-for="phone in branch.telepon">{{ phone }},</span>
                        <br />
                        {{ branch.fax }}
                    </span>
                </div>

            </div>
        </div>
    </div>
</template>

<style lang="postcss" scoped></style>
