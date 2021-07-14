<template>
    <div class="poster-container">
        <div class="inner-poster container">
            <img :src="image" :alt=" 'poster of ' + author " />
            <div class="title">{{title}}</div>  
            <div class="author">{{author}}</div>
            <div class="year">{{year}}</div>
        </div>
    </div>
</template>


<script>
export default {
    name: 'Poster',
    props: {
        image: String,
        title: String,
        author: String,
        year: String,
    }
}
</script>


<style lang="scss" scoped>

</style>
