<template>
    <div class="col-6 col-md-2">
        <div class="inner-more-box">
            <a v-bind:href="url">
                <img class="more-box-img" v-bind:src="image">
            </a>
            <p>{{ text }}</p>
        </div>
    </div>
</template>

<script>
    export default{
        name: 'MoreBox',
        props: {
            imageSrc: String,
            text: String,
            url: String
        },
        data() {
            return {
                image: this.imageSrc,
                text: this.text,
                url: this.url
            }
        }
    }
</script>

<style scoped>
    .inner-more-box{
        text-align: center;
    }

    .more-box-img{
        width: 140px;
        padding: 10px;
        height: 140px;
        border-radius: 20px;
    }
</style>