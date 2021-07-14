<template>

    <div class="main-container">
        <div class="container">
            <div class="row">
                <Poster class="poster-section" v-for="poster in poster" :key='poster.index'
                :poster='poster.image'
                :title='poster.title'
                :author='poster.author'
                :year='poster.year'/>
            </div>
        </div>  
    </div>
</template>


<script>
import Poster from './Poster.vue';

export default {
    name: 'Main',

    components: {
        Poster
    },
    props: {
        poster : Array
    }
}
</script>


<style lang="scss" scoped>
    .main-container {
        
    }
</style>

