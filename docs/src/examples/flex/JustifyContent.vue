<template>
  <div>
    <div
      class="pl-d--flex pl-jc--between bg-gray pl-p--1 pl-mb--2 pl-flex--wrap"
    >
      <div class="pl-m--1">Item 1</div>
      <div class="pl-m--1">Item 2</div>
      <div class="pl-m--1">Item 3</div>
    </div>
    <div
      class="pl-d--flex pl-jc--around bg-gray pl-p--1 pl-mb--2 pl-flex--wrap"
    >
      <div class="pl-m--1">Item 1</div>
      <div class="pl-m--1">Item 2</div>
      <div class="pl-m--1">Item 3</div>
    </div>
    <div
      class="pl-d--flex pl-jc--evenly bg-gray pl-p--1 pl-mb--2 pl-flex--wrap"
    >
      <div class="pl-m--1">Item 1</div>
      <div class="pl-m--1">Item 2</div>
      <div class="pl-m--1">Item 3</div>
    </div>
    <div class="pl-d--flex pl-jc--center bg-gray pl-p--1 pl-flex--wrap">
      <div class="pl-m--1">Item 1</div>
      <div class="pl-m--1">Item 2</div>
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
  opacity: 0.9;
}
.pl-jc--between::before {
  content: ".pl-jc--between";
}
.pl-jc--center::before {
  content: ".pl-jc--center";
}
.pl-jc--around::before {
  content: ".pl-jc--around";
}
.pl-jc--evenly::before {
  content: ".pl-jc--evenly";
}
@media only screen and (max-width: 600px) {
  .pl-d--flex {
    position: relative;
  }
  .pl-d--flex::before {
    display: none;
  }
}
</style>
