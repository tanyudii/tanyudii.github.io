<template>
  <div class="p-4">
    <div
      class="flex flex-row flex-wrap md:flex-row-reverse items-center space-y-4"
    >
      <div class="mx-auto md:w-4/12 md:p-4">
        <img src="/illustration.svg" class="w-64 md:w-96" alt="banner" loading="lazy" />
      </div>
      <div class="md:w-8/12">
        <p class="text-gray-400">Let's introduce my self.</p>
        <div class="text-xl">
          My name is
          <span class="text-blue-400 font-medium">Yudi Hertanto</span>,
          <p>I'm a Web Developer at a Company in Indonesia.</p>
          <p>
            My first Love is Laravel 💓 for Back-end and also Vue.js for
            Front-end 😛
          </p>
          <p>Currently trying to practice with Golang 🚀</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: 'Hi...',
    }
  },
}
</script>
