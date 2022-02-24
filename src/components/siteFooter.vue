<template>
  <div class="main">
    <div class="footer flexDisplayWrap">
      <div class="notHidden rightReserved flexDisplayWrap">
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
      <div class="hiddenRightReserved rightReserved flexDisplayWrap">
        <div><a href="#"><img src="../assets/icon.png" ></a></div>
        <div><p>&copy; 2022 GitHub, Inc.</p></div>
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
    padding-bottom: 50px;
  }
  .footer{
    max-width: 1280px;
    align-content: center;
    justify-content: center;
    margin: auto;
    padding-top: 40px;
    padding-bottom: 10px;
    border-top: 1px solid #333;
  }
  .rightReserved{
    align-items: center;
  }
  .rightReserved p{
    font-size: 12px;
    color: rgba(255, 255, 255, 0.466);
  }
  .rightReserved div{
    margin-left: 10px;
  }
  .links{
    margin: 0 25px;
    justify-content: center;
    align-items: center;
  }
  .links a{
    text-decoration: none;
    color: rgb(0, 153, 255);
    margin-left: 30px;
    font-size: 12px;
  }
  img{
    height: 25px;
    filter: brightness(40%);
  }
  .hiddenRightReserved{
    display: none;
    justify-content: center;
    margin-top: 15px;
  }
  .rightReserved img:hover{
    filter: brightness(100%);
  }
  .links a:hover{
    text-decoration: underline;
  }
  @media screen and (max-width:1012px) {
    .notHidden{
      display: none;
    }
    .footer{
      display: block;
    }
    .hiddenRightReserved{
      display: flex;
    }
  }
</style>