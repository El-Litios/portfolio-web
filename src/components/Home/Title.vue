<template>
  <div class="title mt-4">
      <slot name="title"></slot>
    </div>
</template>

<style lang="css" scoped>
.title {
  text-align: center;
  background-color: rgba(84, 85, 170, 0.4);
  margin-right: 40%;
  margin-left: 40%;
  color: #f5f5dc;
  border-radius: 5%;
}

@media (max-width: 1280px) {
  .title {
    margin-right: auto;
    margin-left: auto;
  }
}
</style>