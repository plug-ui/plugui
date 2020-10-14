<template>
  <div>
    <div class="pl-info-msg">
      <i class="light-icon-info-circle"></i>
      <p>This is an info message.</p>
    </div>
    <div class="pl-success-msg">
      <i class="light-icon-checks"></i>
      <p>This is a success message.</p>
    </div>
    <div class="pl-warning-msg">
      <i class="light-icon-alert-triangle"></i>
      <p>This is a warning message.</p>
    </div>
    <div class="pl-error-msg">
      <i class="light-icon-x"></i>
      <p>This is an error message.</p>
    </div>
    <div class="pl-info-msg pl-transparent-msg pl-shadow__exp-2">
      <i class="light-icon-info-circle"></i>
      <p>This is an info message.</p>
    </div>
    <div class="pl-success-msg pl-transparent-msg pl-shadow__exp-2">
      <i class="light-icon-checks"></i>
      <p>This is a success message.</p>
    </div>
    <div class="pl-warning-msg pl-transparent-msg pl-shadow__exp-2">
      <i class="light-icon-alert-triangle"></i>
      <p>This is an warning message.</p>
    </div>
    <div class="pl-error-msg pl-transparent-msg pl-shadow__exp-2">
      <i class="light-icon-x"></i>
      <p>This is an error message.</p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.pl-info-msg,
.pl-success-msg,
.pl-warning-msg,
.pl-error-msg {
  margin: 1.5rem 0;
  padding: 1rem 1rem;
  font-size: 16px;
  display: flex;
  i {
    font-size: 28px;
    font-weight: 600;
  }
  p {
    margin-top: 6px;
    margin-left: 10px;
  }
}
.pl-info-msg {
  color: #1c587a;
  background-color: #e7f1fa;
  border-top: 5px solid #2b9af3;
}
.pl-success-msg {
  color: #366331;
  background-color: #f3faf2;
  border-top: 5px solid #3e8635;
}
.pl-warning-msg {
  color: #89691c;
  background-color: #fdf7e7;
  border-top: 5px solid #f0ab00;
}
.pl-error-msg {
  color: #7d1007;
  background-color: #faeae8;
  border-top: 5px solid #c9190b;
}
.pl-transparent-msg {
  background: #ffffff;
}
</style>
