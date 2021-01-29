<template>
    <div class="col-md-6">
        <div class="row skill-box">
            <div class="col-4 skill-img-box">
                <img class="skill-img" v-bind:src="image">
            </div>
            <div class="col-8">
                <h2>{{ title }}</h2>
                <p>{{ level }}</p>
                <p>{{ comment }}</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SkillBoxA',
    props: {
        imageSrc: String,
        skillTitle: String,
        skillLevel: String,
        comment: String
    },
    data() {
        return {
            image: this.imageSrc,
            title: this.skillTitle,
            level: this.skillLevel,
            comments: this.comment
        }
    }
}
</script>

<style scoped>
.skill-img{
  height: 100px;
  width: 100px;
  border-radius: 20px;
}

.skill-box{
  height: 180px;
}

.skill-img-box{
  text-align: right;
}
</style>