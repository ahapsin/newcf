<template>
  <div class="flex items-center justify-center w-full  bg-slate-100 h-screen">
    <Card class="w-[25rem]">
      <template #header>
        <div class="flex items-center justify-center w-full p-10">
          <img alt="user header" class=""
               src="https://res.cloudinary.com/doc5sjt7o/image/upload/v1736214034/logo_full_text_zlokhj.png"/>
        </div>
      </template>
      <template #content>
        <div class="flex flex-col gap-y-6">
            <div class="flex flex-col gap-4">
              <Message closable v-if="!username || !email" severity="error" class="mb-2">Validation
                error
              </Message>
<!--              <Message v-if="username && email" severity="success" icon="pi pi-times-circle" class="mb-2">Form is-->
<!--                valid-->
<!--              </Message>-->
              <div class="flex flex-col gap-1">
                <InputText v-model="username" placeholder="Username" aria-label="username" />
<!--                <Message v-if="!username" severity="error" variant="simple" size="small">Username is required</Message>-->
              </div>
              <div class="flex flex-col gap-1">
                <InputText v-model="email" placeholder="Passsword"  type="password" aria-label="password"/>
<!--                <Message v-if="!email" severity="error" variant="simple" size="small">Email is not valid</Message>-->
              </div>
            </div>
        </div>
      </template>
      <template #footer>
        <div class="flex gap-4 mt-10">
          <Button label="Login" class="w-full"/>
          <Button label="Daftar" secondary class="w-full"/>
        </div>
      </template>
    </Card>

  </div>
</template>
<script setup lang="ts">
</script>