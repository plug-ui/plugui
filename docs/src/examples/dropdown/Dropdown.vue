<template>
  <div>
      <div class="pl-dropdown--1 pl-ml--4 pl-mr--4">
          <button class="pl-dropdown--heading">Select Options <i class="light-icon-caret-down"></i></button>
          <ul>
              <li><a href="#">Options 1</a></li>
              <li><a href="#">Options 2</a></li>
              <li><a href="#">Options 3</a></li>
              <li><a href="#">Options 3</a></li>
          </ul>
      </div>
      <div class="pl-dropdown--2 pl-ml--4 pl-mr--4">
          <button class="pl-dropdown--heading">Select Options <i class="light-icon-caret-down"></i></button>
          <ul>
              <li><a href="#">Options 1</a></li>
              <li><a href="#">Options 2</a></li>
              <li><a href="#">Options 3</a></li>
              <li><a href="#">Options 3</a></li>
          </ul>
      </div>
      <div class="pl-dropdown--3 pl-ml--4">
          <button class="pl-dropdown--heading">Select Options</button>
          <ul>
              <li><a href="#">Options 1</a></li>
              <li><a href="#">Options 2</a></li>
              <li><a href="#">Options 3</a></li>
              <li><a href="#">Options 3</a></li>
          </ul>
      </div>
  </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.pl-dropdown--1 {
    font-family: sans-serif;
    position: relative;
    display: inline-block;
    .pl-dropdown--heading {
        border: 1px solid #a4adb8;
        outline: none;
        border-radius: 5px;
        background: #D7DFE8;
        padding: 5px 0.6rem 5px 1rem;
        color: #566D79;
        font-size: 16px;
        cursor: pointer;
        &:focus + ul {
            opacity: 1;
            pointer-events: all;
            transform: translateY(0);
        }
        i {
            font-size: 12px;
            color:#566D79;
        }
    }
    ul {
        width: 200px;
        position: absolute;
        margin-top: 3px;
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        align-items: center;
        list-style: none;
        border-radius: 5px;
        transform: translateY(-10px);
        opacity: 0;
        pointer-events: none;

        transition: all 0.3s ease-in-out;
        li {
            background:#D7DFE8;
            width: 100%;
            height: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            color:#566D79;
            padding: 6px 0;
            cursor: pointer;
            &:hover{
                background: #cbd6e2;
            }
            a {
                color:#566D79;
                text-decoration: none;
            }
        }
        }
    }
.pl-dropdown--2 {
    font-family: sans-serif;
    position: relative;
    display: inline-block;
    .pl-dropdown--heading {
        border: none;
        outline: none;
        border-radius: 5px;
        background: #D7DFE8;
        padding: 5px 0.6rem 5px 1rem;
        color: #566D79;
        font-size: 16px;
        cursor: pointer;
        &:focus {
            border-bottom-left-radius: 0px;
            border-bottom-right-radius: 0px;
        }
        &:focus + ul {
            opacity: 1;
            pointer-events: all;
            transform: translateY(0);
        }
        i {
            font-size: 12px;
            color:#566D79;
        }
    }
    ul {
        width: 100%;
        position: absolute;
        margin-top: 0px;
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        align-items: center;
        list-style: none;
        border-radius: 5px;
        transform: translateY(-10px);
        opacity: 0;
        pointer-events: none;
        transition: all 0.3s ease-in-out;
        li {
            background:#f3f4f7;
            width: 100%;
            height: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            color:#566D79;
            padding: 6px 0;
            cursor: pointer;
            &:hover{
                background:#dfe0e2;
            }
            a {
                color:#566D79;
                text-decoration: none;
            }
        }
        }
    }
.pl-dropdown--3 {
    font-family: sans-serif;
    position: relative;
    display: inline-block;
    width: 200px;
    .pl-dropdown--heading {
        text-align: left;
        width: 100%;
        border: none;
        outline: none;
        border-radius: 2px;
        background: #D7DFE8;
        padding: 5px 0.6rem 5px 1rem;
        color: #566D79;
        font-size: 16px;
        cursor: pointer;
        &:focus + ul {
            opacity: 1;
            pointer-events: all;
            transform: translateY(0);
        }
        i {
            font-size: 12px;
            color:#566D79;
        }
    }
    ul {
        width: 100%;
        position: absolute;
        margin-top: 0px;
        // display: flex;
        flex-direction: column;
        // justify-content: space-around;
        // align-items: center;
        list-style: none;
        border-radius: 5px;
        transform: translateY(-15px);
        opacity: 0;
        pointer-events: none;
        transition: all 0.5s ease-in-out;
        li {
            background:#f3f4f7;
            width: 100%;
            height: 100%;
            display: flex;
            // justify-content: center;
            // align-items: center;
            color:#566D79;
            padding: 6px 0 6px 15px;
            cursor: pointer;
            &:hover{
                background:#dfe0e2;
            }
            a {
                color:#566D79;
                text-decoration: none;
            }
        }
        }
    }
</style>