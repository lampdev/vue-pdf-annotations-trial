<template>
  <div id="app">
    <pdfAnnotate :src="pdf" :toolbar="toolbar" :commentWrapper="commentWrapper"></pdfAnnotate>
  </div>
</template>

<script>

import pdfAnnotate from '@/lib/PdfAnnotate/pdfAnnotate'
import "@/lib/PdfAnnotate/css/toolbar.css";
import "@/lib/PdfAnnotate/css/pdf_viewer.css";

export default {
  name: 'home',
  components: {
    pdfAnnotate
  },
  data(){
    return {
      pdf: 'sample.pdf',
      toolbar: true,
      commentWrapper: true,
    }
  }
}
</script>