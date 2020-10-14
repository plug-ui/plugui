<template>
  <div>
    <div class="pl-d--flex pl-ac--start bg-gray p-p-1 p-mb-2 pl-flex--wrap">
      <div class="pl-m--1 h-200">Item 1</div>
      <div class="pl-m--1 h-100">Item 2</div>
      <div class="pl-m--1">Item 3</div>
    </div>
    <div class="pl-d--flex pl-ac--end bg-gray p-p-1 pl-mb--2 pl-flex--wrap">
      <div class="pl-m--1 h-200">Item 1</div>
      <div class="pl-m--1 h-100">Item 2</div>
      <div class="pl-m--1">Item 3</div>
    </div>
    <div class="pl-d--flex pl-ac--center bg-gray p-p-1 pl-mb--2 pl-flex--wrap">
      <div class="pl-m--1 h-200">Item 1</div>
      <div class="pl-m--1 h-100">Item 2</div>
      <div class="pl-m--1">Item 3</div>
    </div>
    <div
      class="pl-d--flex pl-ac--around bg-gray pl-p--1 pl-mb--2 pl-flex--wrap"
    >
      <div class="pl-m--1 h-200">Item 1</div>
      <div class="pl-m--1 h-100">Item 2</div>
      <div class="pl-m--1">Item 3</div>
    </div>
    <div
      class="pl-d--flex pl-ac--stretch bg-gray pl-p--1 pl-mb--2 pl-flex--wrap"
    >
      <div class="pl-m--1 h-200">Item 1</div>
      <div class="pl-m--1 h-100">Item 2</div>
      <div class="pl-m--1">Item 3</div>
    </div>
    <div
      class="pl-d--flex pl-ac--between bg-gray pl-p--1 pl-mb--2 pl-flex--wrap"
    >
      <div class="pl-m--1 h-200">Item 1</div>
      <div class="pl-m--1 h-100">Item 2</div>
      <div class="pl-m--1">Item 3</div>
    </div>
  </div>
</template>

<script>
export default {};
</script>
<style scoped>
.pl-d--flex {
  position: relative;
  margin-top: 40px;
}
.pl-d--flex::before {
  display: flex;   
    justify-content: center;  
    font-size: 10px;
    font-weight: bold;
    position: absolute;
    left: 95px;
    top: -20px;
    transform: translate(-100%, -50%);
    cursor: pointer;
    background: #607c8a;
    opacity: 0.5;
    transition: all 0.2s ease-in-out;
    color: white;
    height: 26px;
    width: 80px;
    line-height: 26px;
    padding: 0 10px 0 5px;
    margin: 0 10px 10px 0;
    border-radius: 5px;
}
.pl-d--flex:hover::before {
  opacity: 1;
}
.pl-jc--between::before {
  content: "Space Between";
}
.pl-jc--center::before {
  content: "Justify Center";
}
.pl-jc--around::before {
  content: "Space Around";
}
.pl-jc--evenly::before {
  content: "Space Evenly";
}
</style>
