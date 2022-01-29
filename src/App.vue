<template>
  <router-view/>
</template>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  scroll-behavior: smooth;
}
::selection{
  color: #fff;
  background-color: #48bb78;
}
      
/* Scrollbar */

::-webkit-scrollbar {
  display: none;
}
</style>
