<template>
    <div class="section">
        <div class="container">

            <h1 class="title">Les Tres Bessones</h1>
            <div class="columns is-multiline">
                <div v-for="(post, index) in posts" :key="index" class="column is-12-mobile is-6-tablet is-4-desktop" >
                    <Post :title="post.title" :description="post.description" :image="post.image"/>
                    
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
import { ref } from 'vue';
import Post from './Post.vue';
const posts = [
    {
        title: 'Helena',
        description: 'La bessona verd',
        image: 'https://pbs.twimg.com/amplify_video_thumb/1118749914471727104/img/p5QO4Wytd2yz6Hkp.jpg',
    },
    {
        title: 'Anna',
        description: 'La bessona de blau',
        image: 'https://static.filmin.es/images/media/25747/1/card_0_3_1360x765.png'
    },
    {
        title: 'Teresa',
        description: 'La bessona de rosa',
        image: 'https://i.ytimg.com/vi/ftOOygB1iOY/hqdefault.jpg'
    }
]
const colorCard = ref(true);
console.log(posts);


</script>
<style scoped>
.color4 {
    background-color: white;
} .coloret0 {
    background-color: yellowgreen;
} 

.coloret1 {
    background-color: blue;
} 

.coloret2 {
    background-color: violet;
} 

</style>