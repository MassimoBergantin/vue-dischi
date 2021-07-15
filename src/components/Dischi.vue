<template>
<div>
    <img :src="image" :alt="`image of ${title}`" />
    <div class="title">{{title}}</div>
    <div class="author">{{author}}</div>
    <div class="year">{{year}}</div>
</div>
</template>


<script>
export default {
    name: 'Dischi',
    props: {
        image: String,
        title: String,
        author: String,
        year: String
    }
}
</script>


<style lang="scss" scoped>

</style>
 