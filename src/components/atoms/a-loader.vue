<template>
  <div class="loader-item w-16 h-16 rounded-full">
  </div>
</template>

<script>
export default {
    name: "loaderItem"
}
</script>

<style>
     @keyframes spin {
        to { transform: rotate(360deg)}
        
    }
    .loader-item{
        border-top: 8px solid rgba(255, 255, 255, 1);
        border-left: 8px solid rgba(255, 255, 255, 1);
        border-right: 8px solid rgba(255, 255, 255, 0);
        animation: spin 0.575s infinite linear
    }
</style>