<template>
    <section id="skills" class="skills-section">
  <div class="container">
    <div class="row section-title-wrapper">
      <h1 class="col-12">Skills</h1>
    </div>
    <div class="row row-eq-height skill-row-container">
        <SkillBoxA v-bind:imageSrc="skill1.image" v-bind:skillTitle="skill1.title" v-bind:skillLevel="skill1.level" v-bind:comment="skill1.comment" />
        <SkillBoxA v-bind:imageSrc="skill2.image" v-bind:skillTitle="skill2.title" v-bind:skillLevel="skill2.level" v-bind:comment="skill2.comment" />
        <SkillBoxA v-bind:imageSrc="skill3.image" v-bind:skillTitle="skill3.title" v-bind:skillLevel="skill3.level" v-bind:comment="skill3.comment" />
        <SkillBoxA v-bind:imageSrc="skill4.image" v-bind:skillTitle="skill4.title" v-bind:skillLevel="skill4.level" v-bind:comment="skill4.comment" />
    </div>
        <SkillBoxB />
  </div>
</section>
</template>

<script>
import SkillBoxA from './SkillBoxA.vue'
import SkillBoxB from './SkillBoxB.vue'

    export default {
        name: 'Skills',
        components: {
            SkillBoxA,
            SkillBoxB
        },
        data() {
            return {
                skill1: {image: '/java.jpg', title: 'Java', level: '★★★☆☆', comment: 'SpringBootフレームワークを使って開発しています。上流から下流まで開発経験があります。'},
                skill2: {image: '/golang.png', title: 'Go', level: '★☆☆☆☆', comment: '勉強中です。'},
                skill3: {image: '/logo.png', title: 'Vue', level: '★☆☆☆☆', comment: '勉強中です。'},
                skill4: {image: '/aws.png', title: 'AWS', level: '★☆☆☆☆', comment: 'CodePipelineによるCI/CD構築。Lambda'},
            }
        }
    }
</script>