<template>
    <div>
      <h1>Post index</h1>
      <ul>
          <Post 
            v-for="post in posts" 
            :key="post.id" 
            :name="post.title" 
            :id="post.id"
            :content="post.body"
            />
      </ul>
    </div>
</template>

<script>

import axios from 'axios'
import Post from "../components/Post";
export default {
    components: {
        Post
    },
    data(){
        return{
            posts: [],
        }
    },
    async created(){
        try {
            const res = await axios.get('https://jsonplaceholder.typicode.com/posts')
            this.posts = res.data
            
        } catch (error) {
            console.log("Error");
        }
    }
}
</script>
