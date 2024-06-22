<script setup>
    import { ref } from 'vue';
    const currentYear = ref(new Date().getFullYear());
</script>

<template>
    <footer id="site_footer">
        <div class="container">
            <p class="copyright">&copy; {{ currentYear }} Simple Invoice Generator. All rights reserverd.</p>
            <p class="spacer"> • </p>
            <p class="author">Crafted by <a href="https://simplesaint.com" target="_blank" rel="noreferrer">SimpleSaint</a></p>
            <p class="coffee"><a href="https://www.buymeacoffee.com/simplesaint" target="_blank" rel="noreferrer"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" height="35" width="125" class="coffee-button"></a></p>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
    @import '../assets/abstracts.scss'; 

    #site_footer {
        background-image: $gradient-primary;
        color: white;
        text-align: center;
        padding: $spacing-md;
        font-size: $font-size-sm;

        > .container {
            display: flex;
            align-items: center;
            justify-content: center;
            max-width: $container-max;

            @media screen and (max-width: $breakpoint-md){
                flex-direction: column;
            }
        }


        p {
            margin-right: $spacing-sm;
            padding: 0;

            &.coffee {
                margin-left: auto;
            }
        }

        a {
            color: white;
            text-decoration: none;
            font-weight: bold;
        }
    }
</style>