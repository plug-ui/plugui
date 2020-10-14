<template>
  <div>
    <div class="pl-d--flex bg-gray pl-p--1 pl-mb--2 pl-flex--wrap">
      <div class="pl-col--3">Item 1</div>
      <div class="pl-col--3 bg-grey">Item 2</div>
      <div class="pl-col--3">Item 3</div>
      <div class="pl-col--3 bg-grey">Item 4</div>
    </div>
    <div class="pl-d--flex bg-gray pl-p--1 pl-mb--2 pl-flex--wrap">
      <div class="pl-col--4">Item 1</div>
      <div class="pl-col--4 bg-grey">Item 2</div>
      <div class="pl-col--4">Item 3</div>
    </div>
    <div class="pl-d--flex bg-gray pl-p--1 pl-mb--2 pl-flex--wrap">
      <div class="pl-col--6">Item 1</div>
      <div class="pl-col--6 bg-grey">Item 2</div>
    </div>
    <div class="pl-d--flex bg-gray pl-p--1 pl-mb--2 pl-flex--wrap">
      <div class="pl-col--12">Item 1</div>
    </div>
    <div class="pl-d--flex bg-gray pl-p--1 pl-mb--2 pl-flex--wrap">
      <div class="pl-col--5">Item 1</div>
      <div class="pl-col--5 bg-grey">Item 2</div>
      <div class="pl-col--2">Item 3</div>
    </div>
    <div class="pl-d--flex bg-gray pl-p--1 pl-mb--2 pl-flex--wrap">
      <div class="pl-col--3">Item 1</div>
      <div class="pl-col--4 bg-grey">Item 2</div>
      <div class="pl-col--5">Item 3</div>
    </div>
    <div class="pl-d--flex bg-gray pl-p--1 pl-mb--2 pl-flex--wrap">
      <div class="pl-col--8">Item 1</div>
      <div class="pl-col--4 bg-grey">Item 2</div>
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
.pl-d--flex:nth-child(1)::before {
  content: "p-col-3";
}
.pl-d--flex:nth-child(2)::before {
  content: "p-col-4";
}
.pl-d--flex:nth-child(3)::before {
  content: "p-col-6";
}
.pl-d--flex:nth-child(4)::before {
  content: "p-col-12";
}
.pl-d--flex:nth-child(5)::before {
  content: "col5, col5 & col2";
}
.pl-d--flex:nth-child(6)::before {
  content: "col3, col4 & col5";
}
.pl-d--flex:nth-child(7)::before {
  content: "col4 & col8";
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
