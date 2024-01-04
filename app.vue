<template>
  <section class="py-10 md:py-16">
    <div class="container max-w-screen-xl mx-auto px-4">

      <nav class="flex items-center justify-between mb-40">
        <img src="/images/navbar-logo.png" alt="Logo">

        <button @click="confirmDownload"
          class="px-7 py-3 md:px-9 md:py-4 bg-white font-medium md:font-semibold text-gray-700 text-md rounded-md hover:bg-gray-700 hover:text-white transition ease-linear duration-500">Get
          my CV</button>
      </nav>

      <div class="text-center w-full">
        <div class="flex justify-center mb-16 w-full  h-48">
          <img src="/images/image_profile.jpg" class="rounded-full" alt="Image">
        </div>

        <h6 class="font-medium text-gray-600 text-lg md:text-2xl uppercase mb-8">Agamyrat Akmyradov</h6>

        <h1 class="font-normal text-gray-900 text-4xl md:text-7xl leading-none mb-8">passionate web developer</h1>

        <p class="font-normal text-gray-600 text-md md:text-xl mb-16">I have a passion for software. I enjoy creating
          tools that make life easier for people.</p>

      </div>

    </div>

  </section>
</template>

<script setup>
const confirmDownload = () => {
  alert('Not this time!!!')
}
</script>
