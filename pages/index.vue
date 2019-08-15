<template>
  <div class="container">
    <div class="flex flex-wrap">
      <div class="md:w-1/2 px-3">
        <webinar-registration>
          <template v-slot:header>
            <h1 class="text-3xl">
              Welcome to this masterclass
            </h1>
          </template>
          <template v-slot:footer>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
              tempor incididunt ut labore et dolore magna aliqua
            </p>
          </template>
        </webinar-registration>
      </div>
      <div class="md:w-1/2 px-3">
        <webinar-registration />
      </div>
    </div>
  </div>
</template>

<script>
import WebinarRegistration from '~/components/WebinarRegistration.vue'

export default {
  components: {
    WebinarRegistration
  }
}
</script>

<style>
.container {
  @apply min-h-screen mx-auto py-4
}
</style>
