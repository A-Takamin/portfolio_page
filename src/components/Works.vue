<template>
   <section id="works" class="works-section bg-light">
        <div class="container">
            <div class="row section-title-wrapper">
                <h1 class="col-12">Works</h1>
            </div>
            <div class="row works-row">
                <WorksBox v-bind:imageSrc="work1.img" v-bind:description="work1.txt" v-bind:url="work1.url" />
                <WorksBox v-bind:imageSrc="work2.img" v-bind:description="work2.txt" v-bind:url="work2.url" />
            </div>
        </div>
   </section>
</template>

<script>
    import WorksBox from './WorksBox.vue'

    export default {
        name: 'Works',
        components: {
            WorksBox
        },
        data() {
            return {
                work1: {img: '/sample.png', txt: '〇〇なウェブアプリです。あれこれ考えてあれこれを解決することができたらと思い、制作しました。とか言ってますけど別にまだ作っていません。', url: 'javascript:void(0)'},
                work2: {img: '/sample.png', txt: '〇〇なウェブアプリです。あれこれ考えてあれこれを解決することができたらと思い、制作しました。とか言ってますけど別にまだ作っていません。', url: 'javascript:void(0)'}
            }
        }
    }
</script>

<style scoped>
.works-row{
  display: flex;
  justify-content: center;
}
</style>