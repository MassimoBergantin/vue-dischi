<template>
    <div class="poster-container">
        <div class="inner-poster container">
        <img :src="image" :alt=" 'poster of + ' + author" />
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
    .poster-container{
        text-align: center;
        margin-top: 10px;
        
        .inner-poster {
            height: 300px;
            background: #2e3a46;
            padding: 20px;
            line-height: 20px;
                img{
                width: 100%;
            }
            .title{
                font-weight: bold;
                color: #fff;
                padding-top:10px;
            
            }
            .author{
                font-size: 15px;
                color: #808080;
            }
            .year{
                font-size: 12px;
                color: #808080;
            }
        }
        
    }

</style>
