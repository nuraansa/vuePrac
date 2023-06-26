<template>
  <div>
    <h1 class="p-3 pb-0 animate-charcter">Students</h1>
  </div>
</template>

<script>
  
</script>

<style scoped>
.animate-charcter
{
   text-transform: uppercase;
  background-image: linear-gradient(
    -225deg,
    #231557 0%,
    #44107a 29%,
    #ff13f3 67%,
    #ff13f3 78%,
    #231557 100%
  );
  background-size: auto auto;
  background-clip: border-box;
  background-size: 200% auto;
  color: #fff;
  background-clip: text;
  text-fill-color: transparent;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: textclip 3s linear infinite;
  display: inline-block;
      font-size: 90px;
}

@keyframes textclip {
  to {
    background-position: 200% center;
  }
}
</style>