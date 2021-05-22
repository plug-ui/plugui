<template>
  <div class="loaderContainer">
    <div class="pl-loader pl-loader--1">
      <div class="loaderLine"></div>
    </div>

    <div class="pl-loader pl-loader--2">
      <div class="loaderLine"></div>
    </div>

    <div class="pl-loader pl-loader--3">
      <div class="loaderLine"></div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.loaderContainer {
  padding: 0px 40px;
  padding-bottom: 60px;
}

.loaderContainer .pl-loader {
  margin-top: 60px;
}

.pl-loader {
  height: max-content;
  padding: 0px 0px;
  background-color: #607c8a40;
}

//Animation 1

@keyframes loaderAnim1 {
  0% {
    width: 0%;
    margin-left: 0%;
  }
  50% {
    width: 100%;
    margin-left: 0%;
  }
  100% {
    width: 0%;
    margin-left: 100%;
  }
}

.pl-loader--1 .loaderLine {
  background-color: #607c8a;
  height: 4px;
  width: 100%;
  animation: loaderAnim1 2s ease-in-out infinite;
}

//Animation 2

@keyframes loaderAnim2 {
  0% {
    width: 0%;
    margin-left: 0%;
  }
  50% {
    width: 100%;
    margin-left: 0%;
  }
  100% {
    width: 0%;
    margin-left: 100%;
  }
}

.pl-loader--2 .loaderLine {
  background-color: #607c8a;
  height: 4px;
  width: 100%;
  animation: loaderAnim1 2s alternate infinite;
}

//Animation 3

@keyframes loaderAnim3 {
  0% {
    width: 0%;
    margin-left: 0%;
  }
  50% {
    width: 70%;
    margin-left: 15%;
  }
  100% {
    width: 0%;
    margin-left: 100%;
  }
}

.pl-loader--3 .loaderLine {
  background-color: #607c8a;
  height: 4px;
  width: 100%;
  animation: loaderAnim3 2s ease-in-out infinite;
}
</style>