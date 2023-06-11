<template>
  <v-app-bar :elevation="0">
    <template v-slot:append>
      <v-btn icon="mdi-github" size="large"></v-btn>

      <v-btn icon="mdi-linkedin" size="large"></v-btn>

    </template>
  </v-app-bar>
</template>

<script>
export default {};
</script>

<style lang="css" scoped>
.v-toolbar{
  background-color: transparent !important;
  color: beige;
}

.v-btn{
  font-size: 25px !important;
}
</style>