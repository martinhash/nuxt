<template>
  <h1>Post index</h1>
</template>

<script>
export default {
  head(){
    return {
      title: 'post',
      meta: [
        {
          hid: 'description of post',
          name: 'postName',
          content: 'Website post',
        }
      ],
      htmlAttrs: {
        lang: 'es'
      }
    }
  }
}
</script>
