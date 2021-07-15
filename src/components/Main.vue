<template>
<div>
    <Dischi v-for="(dischi, index) in dischi" :key="index" 
    :image='dischi.image'
    :title='dischi.title'
    :author='dischi.author'
    :year='dischi.year'
    />

</div>
</template>


<script>
import Dischi from './Dischi.vue';

export default {
    name: 'Main',

    components: {
        Dischi
    },
    props: {
        dischi : Array
    }
}
</script>


<style lang="scss" scoped>
</style>

