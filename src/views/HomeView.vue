<script setup>
    import Invoice from '../components/Invoice.vue'
    import InvoiceEdit from '../components/InvoiceEdit.vue'
    import PrintButton from '../components/PrintButton.vue'
</script>

<template>
    <main id="home" class="main" data-route="index">
        <section id="main_content" class="container">
            <PrintButton />
            <div class="inner">
                <Invoice />
            </div>
        </section>  
        <aside id="side_content">
            <div class="inner">
                <InvoiceEdit />
            </div>
        </aside>
    </main>
</template>

<style lang="scss" scoped>
    @import '../assets/abstracts.scss';
    
    $page-height: calc(100vh - $header-height);

    #home {  
        display: flex;
        flex-direction: column-reverse;     

        @media screen and (min-width: 992px) {
            flex-direction: row;
        }
    }

    #main_content {
        width: 100%;
        padding-top: var(--spacing-lg);
        padding-bottom: var(--spacing-lg);
        min-height: $page-height;

        @media screen and (min-width: 992px) {
            width: 75%;
            padding-top: var(--spacing-xl);
            padding-bottom: var(--spacing-xl);
        }

        > .inner {
            box-shadow: var(--shadow-default);
            padding: var(--spacing-lg);
        }
    }

    #side_content {
        width: 100%;
        box-shadow: var(--shadow-default);
        padding: var(--spacing-sm);

        @media screen and (min-width: 992px) {
            padding: var(--spacing-lg);
            width: 25%;
            min-height: $page-height;
        }
    }
</style>
