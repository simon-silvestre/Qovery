<template>
    <header>
      <div class="logoContainer">
        <img class="logo" src="@/assets/Logotype.svg" alt="logo de la société">
      </div>
      <div class="banner">
        <div class="text_header" data-aos="fade-down" data-aos-duration="1000">
          <h1>Qovery Engine <span><a class="github-button" href="https://github.com/Qovery/engine" data-size="large" data-show-count="true" aria-label="Star Qovery/engine on GitHub">Star</a></span></h1>
          <p>Abstraction layer to deploy microservices applications on any Cloud provider.</p>
          <p>Qovery Engine is an open-source abstraction layer product that turns easy apps deployment on AWS, GCP, Azure and others Cloud providers.</p>
          <SocialButton />
        </div>
        <div class="img_container" data-aos="fade-left" data-aos-duration="1000">
          <img src="@/assets/aws.svg" alt="">
        </div>
      </div>
    </header>
</template>

<script>
import SocialButton from './SocialButton.vue'

export default {
 components: {
    SocialButton
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  header {
    background-color: #151B2B;
    color: #fff;

    .logoContainer {
      max-width: 1270px;
      margin: 0 auto 0 auto;
      padding: 40px 32px 0 32px;
    }
    .logo {
      width: 158px;
      height: auto;
    }
    .banner {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1270px;
      margin: auto;
      padding: 0 32px 7% 32px;

      .text_header {
        max-width: 470px;
        margin-right: 70px;
        
        h1 {
          font-size: 40px;
          display: flex;

          span {
            margin-left: 20px;
          }
        }
        & p:nth-child(2) {
          font-size: 22px;
          line-height: 35px;
          margin: 20px 0;
          font-weight: 600;
        }
        & p:nth-child(3) {
          font-size: 16px;
          line-height: 24px;
          color: #8686B2;
          margin-bottom: 35px;
        }
      }
      .img_container {
        max-width: 500px; 

        img {
          width: 100%;
        }
      }
    }
  }

  @media screen and (max-width: 800px) {
    .img_container {
      display: none;
    }
    header .banner {
      padding: 0 32px 80px 32px;
    }
    header .banner .text_header {
      margin-right: 0;

      h1 {
        flex-direction: column;
        margin-top: 35px;

        span {
          margin: 20px 0 0 0;
        }
      }
    }
  }
</style>