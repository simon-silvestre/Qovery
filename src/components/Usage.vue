<template>
    <section :style='{ backgroundImage: "url(" + image + ")", }'>
        <h2>Usage</h2>
        <p>Initialize EKS (AWS Kubernetes) and ECR (AWS container registry) on AWS</p>
        <img src="@/assets/texteditor.svg" alt="exemple de code">
        <SocialButton />
    </section>
</template>

<script>
import SocialButton from './SocialButton.vue'

export default {
    components: {
        SocialButton
    },
    data() {
        return {
            image: require('@/assets/Usage_background.svg')
        }
    } 
}
</script>

<style lang="scss" scoped>
    section {
        max-width: 905px;
        background-repeat: no-repeat;
        background-origin: content-box;
        background-position: 95% -5px;
        background-size: 90%;
        height: 100vh;
        margin: 100px auto;
        padding: 0 30px;
        text-align: center;

        h2 {
            color: #454658;
            margin-bottom: 24px;
        }
        img {
            margin-top: 12%;
            width: 100%;        
        }
        .buttons {
            margin: 40px auto;
            text-align: start;
        }
    }
    @media screen and (max-width: 750px) {
        section {
            background-position: 95% 5%;
        }
    }
</style>