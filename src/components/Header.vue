<script setup></script>

<template>
  <header id="site_header">
    <div class="container">
        <h1>Simple Invoice Generator</h1>
    </div>
  </header>
</template>

<style lang="scss" scoped>
    @import '../assets/abstracts.scss'; 

    #site_header {
        background-image: $gradient-primary;
        color: white;

        > .container {
            display: flex;
            align-items: center;
            min-height: $header-height;
            max-width: $container-max;
        }

        h1 {
            font-weight: 300;
            font-size: 4.18rem;
            margin: 0;
        }
    }
</style>