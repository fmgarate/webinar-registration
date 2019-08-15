<template>
  <div class="webinar-registration">
    <div v-if="hasHeader" class="webinar-registration-header">
      <slot name="header" />
    </div>
    <webinar-registration-form />
    <div v-if="hasFooter" class="webinar-registration-footer">
      <slot name="footer" />
    </div>
  </div>
</template>

<script>
import WebinarRegistrationForm from '~/components/WebinarRegistrationForm.vue'

export default {
  name: 'WebinarRegistration',
  components: {
    WebinarRegistrationForm
  },
  computed: {
    hasHeader () {
      return !!this.$slots.header
    },
    hasFooter () {
      return !!this.$slots.footer
    }
  }
}
</script>
