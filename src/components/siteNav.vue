<template>
  <div id="subnavDiv">
    <div class="top flexDisplayWrap"> 
      <div class="leftLinks flexDisplayWrap">
        <div><img class="img" src="../assets/star.png" ></div>
        <div><a href="">guic97</a></div>
        <div><p>/</p></div>
        <div><a href="">site_clone</a></div>
        <div id="repositoryStatus">Public</div>
      </div>
      
      <div class="rightButtons flexDisplayWrap">
        <div>
          <div class="button"><img class="img" src="../assets/star.png" >Pin</div>
        </div>
        <div>
          <div class="button"><img class="img" src="../assets/star.png" >Unwatch (1)</div>
        </div>
        <div>
          <div class="button"><img class="img" src="../assets/star.png" >Fork</div>
        </div>
        <div>
          <div class="button"><img class="img" src="../assets/star.png" >Star (0)</div>
        </div>
      </div>
    </div>
    <div class="shortScreenButtons">
      <div class="shortButtonsTop flexDisplayWrap">
          <div><img class="img" src="../assets/star.png" >0 stars</div>
          <div><img class="img" src="../assets/star.png" >1 forks</div>
      </div>
      <div class="shortButtonsBottom flexDisplayWrap">
          <div class="flexButton"><img class="img" src="../assets/star.png" >Star (0)</div>
          <div class="flexButton"><img class="img" src="../assets/star.png" >Unwatch (1)</div>
      </div>
    </div>
    <div class="subNavbar flexDisplayWrap">
      <div id="firstBar">
        <img class="img" src="../assets/star.png" >
        <p>Code</p>
      </div>
      <div>
        <img class="img" src="../assets/star.png" >
        <p>Issues</p>
      </div>
      <div>
        <img class="img" src="../assets/star.png" >
        <p>Pull requests</p>
      </div>
      <div>
        <img class="img" src="../assets/star.png" >
        <p>Actions</p>
      </div>
      <div>
        <img class="img" src="../assets/star.png" >
        <p>Projects</p>
      </div>
      <div>
        <img class="img" src="../assets/star.png" >
        <p>Wiki</p>
      </div>
      <div>
        <img class="img" src="../assets/star.png" >
        <p>Security</p>
      </div>
      <div>
        <img class="img" src="../assets/star.png" >
        <p>Insights</p>
      </div>
      <div>
        <img class="img" src="../assets/star.png" >
        <p>Settings</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name:'siteNav',
}
</script>

<style scoped>
  #subnavDiv{ 
    max-height: 400px;
    width: 100%;
    border-bottom: 2px solid #222;
  }
  .top{
    padding-top: 16px;
    justify-content: space-between;
    align-content: center;
  }
  .leftLinks{
    justify-content: center;
    align-items: center;
    margin-left: 30px;
  }
  .leftLinks a{
    color: rgb(76, 170, 233);
    font-size: 20px;
    text-decoration: none;
    
  }
  .leftLinks a:hover{
    text-decoration:underline;
  }
  .leftLinks div{
    margin-left: 5px;
  }
  .leftLinks p{
    font-size: 20px;
    color: #888;
  }
  #repositoryStatus{
    border: 1px solid #222;
    color: #666;
    padding: 0 6px;
    border-radius: 15px;
    height: 20px;
    font-size: 12px;
    display: flex;
    align-items: center;
  }
  .rightButtons{
    margin-right: 30px;
  }
  .rightButtons div{
    margin-right: 5px;
    cursor: pointer;
  }
  .rightButtons div,
  .subNavbar div
  {
    display: flex;
    align-items: center;
  }
  .rightButtons img{
    margin-right: 5px;
  }
  .button{
    background-color: rgb(38, 38, 53);
    padding: 5px 12px;
    border-radius: 8px;
    color: blanchedalmond;
    border: 1px solid #444;
  }
  .button:hover, .flexButton:hover{
    background-color: rgb(56, 56, 77);
    border-color: #888;
  }
  .subNavbar{
    margin-top: 10px;
    margin-left: 30px;
  }
  .subNavbar div{
    display: flex;
    flex-wrap: wrap;
    color:rgb(255, 255, 255, 0.897);
    padding: 15px 15px;
    cursor: pointer;
  }
  #firstBar{
    border-bottom: 2px solid rgb(248, 89, 89);
  }
  .subNavbar div:hover{
    border-bottom: 2px solid rgb(71, 70, 70);
  }
  .img{
    margin-right: 5px;
  }
  .shortButtonsTop{
    margin: 0 20px;
    color: rgba(255, 255, 255, 0.712);
  }
  .shortButtonsTop div{
    margin-right: 15px;
    transition: .3s;
  }
  .shortButtonsTop div:hover{
    color: rgba(45, 171, 255, 0.877);
    cursor: pointer;
  }
  .shortButtonsBottom div{
    margin: 0 3px;
    width: 46%;
    display: flex;
  }
  .shortScreenButtons{
    width: 100%;
    display: none;
    flex-direction: column;
  }
  .shortScreenButtons div{
    margin-top: 5px;
    
  }
  .shortScreenButtons > div:nth-child(2n){
    display: flex;
    justify-content: center;
  }
  .flexButton{
    display: flex;
    background-color: rgb(38, 38, 53);
    color: rgba(255, 255, 255, 0.76);
    font-weight: bold;
    justify-content: center;
    padding: 5px;
    border-radius: 5px;
    border: 1px solid #444;
    cursor: pointer;
  }
  @media screen and (max-width:1000px){
    .subNavbar > div:nth-child(9n){
      display: none;
    }
  }
  @media screen and (max-width:900px){
    .subNavbar > div:nth-child(8n){
      display: none;
    }
  }
  @media screen and (max-width:800px){
    .subNavbar > div:nth-child(7n){
      display: none;
    }
  }
  @media screen and (max-width:770px){
    .rightButtons{
      display:none;
    }
    .shortScreenButtons{
      display: flex;
    }
  }
  @media screen and (max-width:720px){
    .subNavbar > div:nth-child(6n){
      display: none;
    }
  }
  @media screen and (max-width:580px){
    .subNavbar > div:nth-child(5n){
      display: none;
    }
  }
  @media screen and (max-width:550px){
    .subNavbar > div:nth-child(5n){
      display: block;
    }
    .subNavbar > div > img{
      display:none;
    }
  }
  
</style>