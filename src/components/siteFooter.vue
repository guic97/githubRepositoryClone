<template>
  <div class="main">
    <div class="footer flexDisplayWrap">
      <div class="rightReserved flexDisplayWrap">
        <div><a href="#"><img src="../assets/icon.png" ></a></div>
        <div><p>&copy; 2022 GitHub, Inc.</p></div>
      </div>
      <div class="links flexDisplayWrap">
        <div><a href="#">Terms</a></div>
        <div><a href="#">Privacy</a></div>
        <div><a href="#">Security</a></div>
        <div><a href="#">Status</a></div>
        <div><a href="#">Docs</a></div>
        <div><a href="#">Contact GitHub</a></div>
        <div><a href="#">Pricing</a></div>
        <div><a href="#">API</a></div>
        <div><a href="#">Training</a></div>
        <div><a href="#">Blog</a></div>
        <div><a href="#">About</a></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name:"siteFooter"
}
</script>

<style scoped>
  .main{
    width: 100%;
  }
  .footer{
    align-content: center;
    align-items: center;
    margin: 0 50px;
    padding: 50px 0;
    border-top: 1px solid #333;
  }
  .rightReserved{
    color:rgba(255, 255, 255, 0.445);
    align-items: center;
  }
  .rightReserved p{
    font-size: 12px;
  }
  .rightReserved div{
    margin-left: 10px;
  }
  .rightReserved img{
    height: 25px;
  }
  .links{
    justify-items: center;
    margin-left: 25px;
  }
  .links a{
    text-decoration: none;
    color: rgb(0, 153, 255);
    margin-left: 40px;
  }
</style>