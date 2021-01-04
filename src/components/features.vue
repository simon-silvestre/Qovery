<template>
    <section>
        <div class="items" v-for="feature in features" :key="feature.title" data-aos="fade" data-aos-duration="1000">
            <img :src="feature.img" alt="icon">
            <h3>{{ feature.title }}</h3>
            <p>{{ feature.paragraphe1 }}</p>
            <br v-if="feature.paragraphe2">
            <p>{{ feature.paragraphe2 }}</p>
            <small><a href="">SEE MORE</a></small>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            features: [
                {
                    img: require('@/assets/feature_1.svg'),
                    title: 'Deploy real world applications',
                    paragraphe1: "Qovery Engine empowers you to deploy complex applications, such as a backend, a frontend, and a database in a very simple way.",
                    paragraphe2: "Servers, networking, security, all is done by the Engine for you."
                },
                {
                    img: require('@/assets/feature_2.svg'),
                    title: 'Resiliency is key',
                    paragraphe1: "Qovery Engine knows when something goes wrong on the deployment of your applications. Qovery Engine is built with resiliency in mind.",
                    paragraphe2: "A transactional engine inspired by what is provided into ACID databases has been developed at the heart of the product to rollback on a consistent and working application version when something goes wrong."
                },
                {
                    img: require('@/assets/feature_3.svg'),
                    title: 'On top of the best tools',
                    paragraphe1: "Qovery Engine does not reinvent the wheel. It takes advantage of the best tools in the Cloud industry, such as Kubernetes, Terraform, and Helm to manage the deployment of the infrastructure and your applications.",
                    paragraphe2: "Servers, networking, security, all is done by the Engine for you."
                },
                {
                    img: require('@/assets/feature_4.svg'),
                    title: 'Extensible',
                    paragraphe1: "Qovery Engine is built to be highly extensible. Adding the support of a Cloud provider or a Continuous Integration platform is as simple as implementing a simple programmatic interface."
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    section {
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
        margin: 100px auto 0 auto;
        padding: 0 30px 100px 30px;
        max-width: 1060px;

        .items {
            max-width: 400px;
            font-size: 16px;
            margin-top: 65px;
            color: #454658;
            line-height: 150%;

            img {
                height: 160px;
            }
            h3 {
                margin: 24px 0;
            }
            small {
                display: inline-block;
                font-weight: bold;
                margin-top: 12px;
                
                a {
                    text-decoration: none;
                    color: #6578C0;
                }
            }
            &:nth-child(1), &:nth-child(3) {
                margin-right: 30px;
            }
        }
    }
    @media screen and (max-width: 905px) {
       section {
            justify-content: center;

          .items {
              text-align: center;
          }
       }
    }
    @media screen and (max-width: 700px) {
        section .items {
            &:nth-child(1), &:nth-child(3) {
                margin-right: 0px;
            }
        }
    }
</style>