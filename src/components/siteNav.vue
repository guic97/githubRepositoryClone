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
      <div id="shortScreenButtons">
        <div>
          <div class="button"><img class="img" src="../assets/star.png" >Star (0)</div>
        </div>
        <div>
          <div class="button"><img class="img" src="../assets/star.png" >Unwatch (1)</div>
        </div>
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
    max-width: 100%;
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
    color: rgb(0, 153, 255);
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
  }
  .rightButtons{
    margin-right: 30px;
  }
  .rightButtons div{
    margin-right: 5px;
    cursor: pointer;
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
  .button:hover{
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
  .subNavbar img{
    margin-right: 5px;
  }
  #shortScreenButtons{
    display: none;
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
  @media screen and (max-width:720px){
    .subNavbar > div:nth-child(6n){
      display: none;
    }
    .rightButtons{
      display:none;
    }
    #shortScreenButtons{
    display: flex;
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