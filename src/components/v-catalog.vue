<template>
    <div class="v-catalog">
        <h1>Catalog</h1>
        <div class="v-catalog__list">
            <v-catalog-item
                v-for="product in products"
                v-bind:key="product.article"
                v-bind:product_data="product"
             />
        </div>
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
            return {
                "products": [
                    {
                        image: "1.jpg",
                        name: "T-shirt 1",
                        price: 2100,
                        article: "T1",
                        available: true,
                        category: "Мужские"
                    },
                    {
                        image: "2.jpg",
                        name: "T-shirt 2",
                        price: 3150,
                        article: "T2",
                        available: true,
                        category: "Женские"
                    },
                    {
                        image: "3.jpg",
                        name: "T-shirt 3",
                        price: 4200,
                        article: "T3",
                        available: false,
                        category: "Женские"
                    },
                    {
                        image: "4.jpg",
                        name: "T-shirt 4",
                        price: 5300,
                        article: "T4",
                        available: true,
                        category: "Мужские"
                    },
                    {
                        image: "5.jpg",
                        name: "T-shirt 5",
                        price: 6500,
                        article: "T5",
                        available: false,
                        category: "Женские"
                    },
                    {
                        image: "6.jpeg",
                        name: "T-shirt 6",
                        price: 8700,
                        article: "T6",
                        available: true,
                        category: "Женские"
                    }
  ]
            }
        },
        computed: {

        }
    }
</script>

<style lang="scss">
    .v-catalog {
        &__list {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            align-items: center;
        }
    }
</style>