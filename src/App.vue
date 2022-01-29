<template>
  <router-view/>
</template>

<style>
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
  width: 5px;
}
      
::-webkit-scrollbar-track {
  background: #f1f1f1;
}
      
::-webkit-scrollbar-thumb {
  background: #48bb78;
}
::-webkit-scrollbar-thumb:hover {
  background: #2da15e;
}
</style>
