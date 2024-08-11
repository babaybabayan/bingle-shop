<template>
  <v-row>
    <v-col cols="8" class="frame-content"> <products></products> </v-col>
    <v-col cols="4"> Orders </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>

<style scoped>
.frame-content {
  overflow-y: auto;
}
</style>
