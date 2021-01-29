<template>
    <section id="more">
        <div class="container">
            <div class="row section-title-wrapper">
                <h1 class="col-12">More?</h1>
            </div>
            <div class="row">
                <MoreBox v-bind:imageSrc="more1.img" v-bind:text="more1.txt" v-bind:url="more1.url" />
                <MoreBox v-bind:imageSrc="more2.img" v-bind:text="more2.txt" v-bind:url="more2.url" />
                <MoreBox v-bind:imageSrc="more3.img" v-bind:text="more3.txt" v-bind:url="more3.url" />
                <MoreBox v-bind:imageSrc="more4.img" v-bind:text="more4.txt" v-bind:url="more4.url" />
                <MoreBox v-bind:imageSrc="more5.img" v-bind:text="more5.txt" v-bind:url="more5.url" />
                <MoreBox v-bind:imageSrc="more6.img" v-bind:text="more6.txt" v-bind:url="more6.url" />
                <MoreBox v-bind:imageSrc="more7.img" v-bind:text="more7.txt" v-bind:url="more7.url" />
                <MoreBox v-bind:imageSrc="more8.img" v-bind:text="more8.txt" v-bind:url="more8.url" />
                <MoreBox v-bind:imageSrc="more9.img" v-bind:text="more9.txt" v-bind:url="more9.url" />
                <MoreBox v-bind:imageSrc="more10.img" v-bind:text="more10.txt" v-bind:url="more10.url" />
                <MoreBox v-bind:imageSrc="more11.img" v-bind:text="more11.txt" v-bind:url="more11.url" />
                <MoreBox v-bind:imageSrc="more12.img" v-bind:text="more12.txt" v-bind:url="more12.url" />

            </div>
        </div>
    </section>
</template>

<script>
    import MoreBox from './MoreBox.vue'

    export default {
        name: 'More',
        components: {
            MoreBox
        },
        data() {
            return {
                more1: {img: '/forkwell.png', txt: 'Forkwell', url: 'https://portfolio.forkwell.com/@A-Takamin'},
                more2: {img: '/github.png', txt: 'Github', url: 'https://github.com/A-Takamin'},
                more3: {img: '/darts.png', txt: '趣味：ダーツ', url: 'javascript:void(0);'},
                more4: {img: '/travel.jpg', txt: '趣味：旅行', url: 'javascript:void(0);'},
                more5: {img: '/narou.jpg', txt: '趣味：なろう', url: 'javascript:void(0);'},
                more6: {img: '/mintos.png', txt: 'pcOS：mintOS', url: 'javascript:void(0);'},
                more7: {img: '/vscode.jpg', txt: 'エディタ：vscode', url: 'javascript:void(0);'},
                more8: {img: '/sample.png', txt: 'hoge', url: 'javascript:void(0);'},
                more9: {img: '/sample.png', txt: 'hoge', url: 'javascript:void(0);'},
                more10: {img: '/sample.png', txt: 'hoge', url: 'javascript:void(0);'},
                more11: {img: '/sample.png', txt: 'hoge', url: 'javascript:void(0);'},
                more12: {img: '/sample.png', txt: 'hoge', url: 'javascript:void(0);'},
            }
        }
    }
</script>