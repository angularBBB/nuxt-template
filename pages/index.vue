<template>
  <Tutorial />
</template>

<script setup lang="ts">
import { useFetch,useAsync } from "@nuxtjs/composition-api"

useAsync(()=>{
  console.log(123);

})

useFetch(() => {
  console.log(456);

})
</script>
