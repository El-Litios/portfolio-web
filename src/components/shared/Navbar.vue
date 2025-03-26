<template>
  <v-app-bar color="primary" :elevation="100">
    <template v-slot:append>
      <v-btn icon="mdi-github" href="https://github.com/El-Litios" size="large"></v-btn>
      <v-btn icon="mdi-linkedin" href="https://www.linkedin.com/in/cguzmanr/" size="large"></v-btn>
      <v-btn icon="mdi-email" href="mailto:carlosguzmanrojas00@gmail.com" size="large"></v-btn>

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