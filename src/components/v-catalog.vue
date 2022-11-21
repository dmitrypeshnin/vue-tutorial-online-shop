<template>
    <div class="v-catalog">
        <h1>Catalog</h1>
        <VCatalogItem />
    </div>
</template>

<script>
    import VCatalogItem from './v-catalog-item'
import vCatalogItem from './v-catalog-item.vue';

    export default {
        name: 'v-catalog',
        components: {
    VCatalogItem,
            vCatalogItem,
        },
        props: {},
        data() {
            return {}
        },
        computed: {

        }
    }
</script>

<style>

</style>