<template>
  <h1>About page</h1>
</template>

<script>
export default {
  head(){
    return {
      title: 'About us',
      meta: [
        {
          hid: 'description of about',
          name: 'aboutName',
          content: 'Website about',
        }
      ],
      htmlAttrs: {
        lang: 'es'
      }
    }
  }
}
</script>
