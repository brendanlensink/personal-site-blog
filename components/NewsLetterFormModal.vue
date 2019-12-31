<template>
    <news-letter-form />
</template>
<script>
import NewsLetterForm from '~/components/NewsLetterForm'
export default {
  components: { NewsLetterForm },
  computed: {
    title() {
      return (
        this.$siteConfig.newsletter.heading || 'Subscribe to Our Newsletter'
      )
    }
  }
}
</script>

<style lang="scss">
.newsletter-modal {
  .field.has-addons {
    justify-content: center;
  }
}
</style>
