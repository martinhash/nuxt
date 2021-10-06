<template>
<nuxt-link :to="'/' + id">
    <div>
        <p>
            {{id}}. {{name}}
            <br>
            {{content}}
        </p>
    </div>
</nuxt-link>
</template>

<script>
export default {
    name: 'Post',
    props: ['id', 'name', 'content']
}
</script>