<template>
  <NuxtLayout class="scroll-smooth">
    <NuxtLoadingIndicator color="#2F54CB" />
    <NuxtPage include="index"></NuxtPage>
    <NuxtSnackbar />
  </NuxtLayout>
</template>

<script setup>

const confirmDownload = () => {
  alert('Not this time!!!')
}


useHead({
  htmlAttrs: { lang: 'en' },
  title: 'Agamyrat Akmyradov',
  meta: [
    {
      name: "title",
      content: 'Agamyrat Akmyradov',
    },
    {
      name: "description",
      content: 'passionate web developer',
    },
  ],
  link: [
    {
      rel: 'icon',
      type: 'image/x-icon',
      href: '/icon.ico',
    },
  ],
});

</script>
