<script setup>
    const printInvoice = () => {
        window.print()
    }
</script>

<template>
    <button class="print-button" @click="printInvoice">Print</button>
</template>

<style lang="scss" scoped>
    .print-button {
        background-color: var(--color-primary);
        color: white;
        padding: var(--spacing-sm) var(--spacing-lg);
        border: none;
        border-radius: var(--border-radius);
        cursor: pointer;
        font-size: 1.25rem;
        margin-bottom: var(--spacing-lg);
    }
</style>