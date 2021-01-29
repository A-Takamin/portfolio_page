<template>
    <div class="row skill-box">
            <div class="col-md-2 col-4 skill-img-box">
                <img class="skill-img" v-bind:src="image">
            </div>
        <div class="col-md-10 col-8">
            <h2>{{ title }}</h2>
            <p>{{ text1 }}</p>
            <p>{{ text2 }}</p>
            <p>{{ text3 }}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SkillBoxB',
    data() {
        return {
            image: '/intelligence.png', 
            title: 'Others', 
            text1: '業務経験あり：Docker, Git, ', 
            text2: '使用経験あり：', 
            text3: '資格：Java Gold, AWS CP, TOEIC 830',            
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