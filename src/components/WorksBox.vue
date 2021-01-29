<template>
        <div class="col-md-5 work-box">
            <a v-bind:href="url">
                <img class="work-img" v-bind:src="image">
            </a>
            <p>{{ description }}</p>
        </div>
</template>

<script>
export default {
    name: 'WorksBox',
    props: {
        imageSrc: String,
        description: String,
        url: String
    },
    data() {
        return {
            image: this.imageSrc,
            description: this.description,
            url: this.url
        }
    }
}
</script>

<style scoped>
    .work-box{
        text-align: center;
    }
    .work-img{
        width: 200px;
        border-radius: 20px;
    }
</style>