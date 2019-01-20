<template>
    <div class="header">
      <router-link  :to="{name:'root'}">
        <img src="../assets/cnodejs_light.svg" alt="">
      </router-link>
      <input type="search">
      <ul>
        <li><a href="#">首页</a></li>
        <li><a href="#">新手入门</a></li>
        <li><a href="#">API</a></li>
        <li><a href="#">关于</a></li>
        <li><a href="#">注册</a></li>
        <li><a href="#">登录</a></li>
      </ul>
    </div>
</template>

<script>
    export default {
        name: "Header"
    }
</script>

<style scoped>
.header{
  background-color:#5a5555 ;
  height: 50px;
}
img{
  max-width: 120px;
  margin-left: 50px;
  margin-top: 10px;
    float: left;

}
input {
  background: #888 url("../assets/search.png") 4px 4px no-repeat;
    color: #666;
    border: none;
    outline: none;
    width: 233px;
    height: 28px;
    border-radius: 15px;
    float: left;
    margin-top: 11px;
    margin-left: 20px;
    transition: all 0.5s;
    text-indent: 22px;
  }
  input:hover {
    background: #fff url("../assets/search.png") 4px 4px no-repeat;
  }
  input::-webkit-search-cancel-button{
    display: none;
  }
  input[type=search]::-ms-clear{
    display: none;
  }
  ul{
    list-style: none;
    float: right;
    margin: 4px;
  }
  li{
    display: inline-block;
    padding: 10px 15px;
  }
  a{
    text-decoration: none;
    color: #ccc;
    font-size: 14px;
    text-shadow: nonr;
  }
</style>
