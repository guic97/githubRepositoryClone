<template>
  <header class='header flexDisplayWrap'>
    <nav class='flexDisplayWrap'>
      <ul class='flexDisplayWrap' id="leftNav">
        <li><div id="menu">Menu</div></li>
        <li><a href="#"><img src="../assets/icon.png"></a></li>
        <ul class='flexDisplayWrap'>
          <li><input type="text" placeholder="Search or jump to..."></li>
          <li><a href="#">Pull</a></li>
          <li><a href="#">Issues</a></li>
          <li><a href="#">Marketplace</a></li>
          <li><a href="#">Explore</a></li>
        </ul>
      </ul>
      <ul class='flexDisplayWrap' id="rightNav">
        <li><a href="#">Sino</a></li>
        <ul class='flexDisplayWrap'>
          <li><a href="#"><h1>+</h1></a></li>
          <li><a href="#" ><img src="../assets/foto.jpg" id="profilePhoto"></a></li>
        </ul>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name:"siteHeader",
}
</script>

<style scoped>
  
  header{
    background-color: rgb(25, 30, 37);
    justify-content: space-between;
    align-items: center;
    padding: 16px;
  }
  ul li, ul a{
    margin-right: 12px;
    text-decoration: none;
    color: rgba(255, 255, 255, 0.897);
    font-weight: bold;
    display: flex;
    align-items: center;
  }
  a img{
    width: 32px;
  }
  nav {
    justify-content: space-between;
    width: 100%;
  }
  a img:hover{
    filter:brightness(70%);
  }
  h1{
    font-size: 25px;
  }
  a:hover{
    color: rgb(190, 189, 189);
  }
  #leftNav:first-child{
    margin-left: 5px;
  }
  input{
    color:white;
    background-color:rgb(16, 19, 24);
    border-radius: 5px;
    padding: 4px 0;
    padding-left: 12px;
    border: 1px solid rgb(58, 57, 57);
  }
  #profilePhoto{
    border: 1px solid #555;
    border-radius: 30px;
    width: 20px;
  }
  #menu{
    display: none;
  }
  @media screen and (max-width:768px){
    nav ul ul{
      display: none;
    }
    #menu{
      display: block;
    }
    nav #leftNav{
      width: 55%;
      justify-content: space-between;
    }
  }
</style>