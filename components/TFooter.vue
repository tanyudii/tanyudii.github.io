<template>
  <div class="p-4 pt-0">
    <div class="border-t pt-3 border-gray-100">
      <div class="grid grid-cols-1 md:grid-cols-12 gap-3">
        <div class="md:col-span-4">
          <p class="text-gray-400">Get in touch</p>
          <a :href="email.mailto" class="text-lg text-gray-500 font-semibold">{{
            email.label
          }}</a>
        </div>
        <div class="md:col-span-8">
          <p class="text-gray-400">Follow me on</p>
          <div class="flex flex-wrap flex-col md:flex-row md:space-x-8">
            <a
              v-for="(social, index) in socials"
              :key="index"
              :href="social.url"
              class="text-lg text-gray-500 font-semibold"
              >{{ social.title }}</a
            >
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      email: {
        label: 'hi@tanyudii.me',
        mailto: 'mailto:hi@tanyudii.me?subject=Hi Yudi',
      },
      socials: [
        { title: 'Github', url: 'https://github.com/tanyudii' },
        { title: 'Instagram', url: 'https://instagram.com/tanyudii' },
        { title: 'Linkedin', url: 'https://www.linkedin.com/in/tanyudii/' },
        { title: 'Twitter', url: 'https://twitter.com/tanyudii' },
      ],
    }
  },
}
</script>
