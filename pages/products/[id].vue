<template>
  <div>
    <p>Product details for {{ id }}</p>
    <p>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Est fugit rerum
      laborum totam voluptate modi, ipsam quas. Blanditiis, delectus ullam omnis
      beatae odio quos sapiente, esse quia quaerat deleniti odit.
    </p>
  </div>
</template>

<script setup lang="ts">
const { id } = useRoute().params;
</script>

<style scoped></style>
