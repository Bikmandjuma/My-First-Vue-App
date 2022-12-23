<template>
  <button @click='increment'>counting : {{count}}</button>
</template>

<script>
export default {
  data(){
    return {
      count: 2
    }
  }
}
</script>
