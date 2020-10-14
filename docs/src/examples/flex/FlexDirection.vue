<template>
  <div>
    <div class="pl-d--flex pl-flex--row bg-gray pl-p--1 pl-mb--2 pl-flex--wrap">
      <div class="pl-m--1">Item 1</div>
      <div class="pl-m--1">Item 2</div>
      <div class="pl-m--1">Item 3</div>
    </div>
    <div
      class="pl-d--flex pl-flex--row-reverse bg-gray pl-p--1 pl-mb--2 pl-flex--wrap"
    >
      <div class="pl-m--1">Item 1</div>
      <div class="pl-m--1">Item 2</div>
      <div class="pl-m--1">Item 3</div>
    </div>
    <div
      class="pl-d--flex pl-flex--column bg-gray pl-p--1 pl-mb--2 pl-flex--wrap"
    >
      <div class="pl-m--1">Item 1</div>
      <div class="pl-m--1">Item 2</div>
      <div class="pl-m--1">Item 3</div>
    </div>
    <div
      class="pl-d--flex pl-flex--column-reverse bg-gray pl-p--1 pl-mb--2 pl-flex--wrap"
    >
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
  opacity: 1;
}
.pl-flex--row::before {
  content: "Row (Default)";
}
.pl-flex--row-reverse::before {
  content: "Row Reverse";
}
.pl-flex--column::before {
  content: "Column";
}
.pl-flex--column-reverse::before {
  content: "Column Reverse";
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
