<template>
    <div class="section">
        <div class="container">

            <h1 class="title">Les Tres Bessones</h1>
            <div class="columns is-multiline">
                <div v-for="post in posts" class="column is-12-mobile is-6-tablet is-4-desktop">
                    <Post :title="post.title" :description="post.description" :image="post.image" :style="{ 'background-color': post.activeColor}"/>                    
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
        description: 'La bessona que sempre té molta gana',
        image: 'https://pbs.twimg.com/amplify_video_thumb/1118749914471727104/img/p5QO4Wytd2yz6Hkp.jpg',
        activeColor: '#69BF76',
    },
    {
        title: 'Anna',
        description: 'La bessona més romàntica i dolça',
        image: 'https://static.filmin.es/images/media/25747/1/card_0_3_1360x765.png',
        activeColor: '#5D92D4',
    },
    {
        title: 'Teresa',
        description: 'La bessona més decidida',
        image: 'https://i.ytimg.com/vi/ftOOygB1iOY/hqdefault.jpg',
        activeColor: '#DD6688',
    }
]
const colorCard = ref(true);
console.log(posts);


</script>
<style scoped>
.color4 {
    background-color: white;
}

</style>