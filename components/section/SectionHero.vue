<template>
    <div class="flex bg-primary-50/10 bg-[url('/p1.png')] bg-cover md:bg-right">
        <div class="relative py-44 pb-20 md:py-[200px] p-10 md:ps-20 flex flex-col  gap-y-4 w-full md:w-1/2">
            <span class="text-2xl md:text-5xl ">
                <div class="flex flex-col leading-tight font-semibold">
                    <div class="text-orange-500 font-bold">Semangat Baru </div>
                    <div class="text-primary ">Dalam Usaha Anda</div>
                </div>
            </span>
            <span class="text-xs md:text-lg text-muted-color w-3/4 md:w-3/4 leading-normal">
                Kami menawarkan berbagai solusi untuk permasalahan anda mulai dari kredit dengan suku bunga yang
                kompetitif..
            </span>
            <InputGroup rounded>
                <InputText placeholder="email bisnis anda" class="w-full" />
                <Button class="w-1/3 md:w-1/2">
                    <Icon name="line-md:external-link" />
                </Button>
            </InputGroup>
            <div class="absolute left-10">
                <NuxtImg src="" />
            </div>
        </div>

    </div>
</template>
