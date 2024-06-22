<script setup>
import From from './From.vue'
</script>

<template>
    <section id="invoice">
        <header class="invoice-header">
            <div class="inner">
                <h2 class="invoice-heading">Invoice</h2>
                <From />
            </div>
        </header>
    </section>
</template>

<style lang="scss" scoped>
    .invoice-header {
        display: flex;
        justify-content: space-between;
        align-items: flex-start;
        margin-bottom: var(--spacing-lg);
        border-bottom: 5px solid var(--color-dark-gray);
    }
    .invoice-heading {
        font-size: 3.75rem;
        margin: 0;
    }
</style>