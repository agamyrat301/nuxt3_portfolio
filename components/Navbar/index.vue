<template>
    <nav class="flex items-center justify-between mb-40">
        <h1 class="font-semibold text-lg"><code> {{ title }}</code> </h1>

        <button @click="confirmDownload"
            class="px-7 py-3 md:px-9 md:py-4 bg-white font-medium md:font-semibold text-gray-700 text-md rounded-md hover:bg-gray-700 hover:text-white transition ease-linear duration-500">Get
            my CV</button>
    </nav>
</template>

<script setup>
const confirmDownload = () => {
    const filePath = '/files/RESUME.pdf';

    // Construct the full URL using the publicPath provided by Vue CLI
    const fileUrl = `http://localhost:3000${filePath}`;

    // Create a hidden link element
    const link = document.createElement('a');
    link.href = fileUrl;
    link.setAttribute('download', 'resume.pdf'); // Set the desired file name

    // Append the link to the document and trigger the click event
    document.body.appendChild(link);
    link.click();

    // Remove the link from the document
    document.body.removeChild(link);

}
const title = ref('<Agamyrat/>')


</script>
