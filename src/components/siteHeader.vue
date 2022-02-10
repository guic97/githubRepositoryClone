<template>
  <header class='header'>
    <nav>
      <ul id="leftNav">          
        <li><a href="#"><img src="../assets/icon.png"></a></li>
        <li><input type="text" placeholder="Search or jump to..."></li>
        <ul>
          <li><a href="#">Pull requests</a></li>
          <li><a href="#">Issues</a></li>
          <li><a href="#">Marketplace</a></li>
          <li><a href="#">Explore</a></li>
        </ul>
      </ul>
    </nav>
    <nav>
      <ul id="rightNav">
        <li><a href="#">Sino</a></li>
        <li><a href="#"><h1>+</h1></a></li>
        <li><a href="#" ><img src="../assets/foto.jpg" id="profilePhoto"></a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name:"siteHeader",
  data(){
    return{
      
    }
  }
}
</script>

<style scoped>
  header{
    background-color: rgb(25, 30, 37);
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
    padding: 16px;
  }
  nav ul{
    display: flex;
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
    width: 32px
  }
  h1{
    font-size: 25px;
  }
  a:hover{
    color: rgb(190, 189, 189);
  }
  #leftNav:first-child{
    margin-left: 15px;
  }
  input{
    color:white;
    background-color:rgb(16, 19, 24);
    border-radius: 5px;
    padding: 4px 0;
    padding-left: 12px;
    border: 1px solid rgb(58, 57, 57);
    width: 250px;
  }
  #profilePhoto{
    border: 1px solid #555;
    border-radius: 30px;
  }
</style>