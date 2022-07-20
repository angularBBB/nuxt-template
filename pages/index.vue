<template>
  <div>123</div>
</template>

<script setup lang="ts">
import { onMounted } from "vue"
import { useFetch,useAsync } from "@nuxtjs/composition-api"


onMounted(()=>{
  console.log('onMounted'); // not log
})

useAsync(()=>{
  console.log(123);

})

useFetch(() => {
  console.log(456);

})
</script>
