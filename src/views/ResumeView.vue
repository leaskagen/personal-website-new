<template>
  <div class="resume">
    <vue-pdf-embed :source="pdfSource" width="100%" height="100vh"/>
    <embed src="@/assets/resume.pdf" type="application/pdf" width="100%" height="100vh"/>
  </div>
</template>

<style>
embed {
  width: 100%;
  height: 100%;
}
</style>

<script>
import VuePdfEmbed from 'vue-pdf-embed'

export default {
  name: 'ResumeView',
  components: {
    VuePdfEmbed
  }, data() {
    return {
      pdfSource: '@/assets/resume.pdf'
    }
  }
}
</script>