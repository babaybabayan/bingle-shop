<template>
  <v-row>
    <v-col v-for="(product, index) in products" cols="2">
      <v-card :title="product.title" :ripple="true">
        <v-card-actions>
          ini gambar
          <!-- <v-img
            :src="require(`@/assets/images/products/${product.thumbnail}`)"
          >
          </v-img> -->
        </v-card-actions>
        <v-card-text align="center" class="product-title">
          {{ product.title }}
        </v-card-text>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  data() {
    return {
      products: [
        {
          id: 1,
          title: 'Asus Zenfone',
          thumbnail: 'asus-zenfone.png',
          price: 2000000,
          categoryId: 1,
        },
      ],
    }
  },
}
</script>

<style scoped>
.product-title {
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}
</style>
