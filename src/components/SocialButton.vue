<template>
    <div class="buttons">
        <a href="https://github.com/Qovery"><img class="github" src="@/assets/github.svg" alt="">See on Github</a>
        <a href="https://discord.com/invite/Bed5FRa"><img src="@/assets/discord.svg" alt="">Join us on Discord</a>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss">
    .buttons {
        width: fit-content;
        display: flex;
        justify-content: space-between;
        a {
            width: fit-content;
            display: flex;
            align-items: center;
            padding: 9px 16px;
            border-radius: 3px;
            text-decoration: none;
            font-size: 14px;
            font-weight: 600;

            color: #fff;

            &:nth-child(1) {
                background-color: #454658;
                margin-right: 20px;
            }
            &:nth-child(2) {
                background-color: #6578C0;
            }

            img {
                width: 16px;
                margin-right: 7px;
            }
            .github {
                width: 19px;
            }
        }
    }
</style>