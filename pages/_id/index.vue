<template>
    <h1>{{post.id}} - {{post.title}}</h1>
</template>

<script>
import axios from "axios";
export default {
    data(){
        return {
            post: {}
        }
    },
    async created(){
        try {
            const res = await axios.get(`https://jsonplaceholder.typicode.com/posts/${this.$route.params.id}`)
            this.post = res.data
        } catch (error) {
            
        }
    }
}
</script>