<template>
    <section>
        <h2>How does it work ?</h2>
        <p>
            Qovery Engine is an open-source abstraction layer product that turns easy apps deployment on AWS, GCP, Azure and others Cloud providers. 
            The Qovery Engine is coded in Rust and takes advantage of Terraform, Helm, Kubectl, Docker to manage resources.
        </p>
        <img src="@/assets/work.svg" alt="fonctionnement du systeme">
    </section>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
    section {
        margin: 100px auto;
        padding: 0 30px;
        max-width: 855px;
        text-align: center;

        h2 {
            color: #454658;
            margin-bottom: 24px;
        }
        p {
            line-height: 24px;
        }
        img {
            width: 100%;
            margin-top: 32px;
        }
    }
</style>