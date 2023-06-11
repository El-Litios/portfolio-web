<template>
  <v-carousel hide-delimiters :show-arrows="false">
    <v-carousel-item
      gradient="black"
      src="src/assets/images/carousel-image.jpg"
      cover
    >
      <v-sheet>
        <div class="text-center fill-height justify-center align-center">
          <div class="text-h1">Carlos Guzmán</div>
          <div>
            <v-btn>
              CV
              <v-icon end icon="mdi-download"></v-icon>
            </v-btn>
          </div>
        </div>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>
</template>

<script>
export default {
  setup() {},
};
</script>

<style lang="css" scoped>
.v-sheet {
  background-color: transparent;
}

.text-h1 {
  margin-top: 10%;
  font-weight: bold;
  color: #f5f5dc;
}

.v-btn{
  background-color: rgba(127, 93, 185, 0.9);
  color: #f5f5dc;
  font-weight: bold;
}

@media (max-width: 1000px) {
  .text-h1 {
    margin-top: 25%;
    text-align: center;
  }
}
</style>