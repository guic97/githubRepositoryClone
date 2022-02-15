<template>
  <div class="main flexDisplayWrap">
    <section class="section">
      <div class="topButtons flexDisplayWrap">
        <div class="leftButtons flexDisplayWrap">
          <div class="button">
            <div><img class='img' src="../assets/star.png"></div>
            <div><p>master</p></div>
          </div>
          <div class="buttonTwo flexDisplayWrap">
            <div><img class='img' src="../assets/star.png"><h3>1</h3></div>
            <p>branch</p>
          </div>
          <div class="buttonTwo flexDisplayWrap">
            <div><img class='img' src="../assets/star.png"><h3>0</h3></div>
            <p>tags</p>
          </div>
        </div>
        <div class="rightButtons flexDisplayWrap">
          <div class="button">
            <p>Go to file</p>
          </div>
          <div class="button">
            <p>Add file</p>
          </div>
          <div id='codeButton' class="button">
            <p>Code</p>
          </div>
        </div>
      </div>
      <div class="repository">
        <div class="repositoryName flexDisplayWrap">
          <div class="leftContent flexDisplayWrap">
            <div class="photoDiv flexDisplayWrap">
              <a href="#" ><img src="../assets/foto.jpg"></a>
            </div>
            <div>
              <a href="#">guic97</a>
            </div>
            <div>
              <a href="#">current commit</a>
            </div>
          </div>
          <div class="rightContent flexDisplayWrap">
            <div>
              <p>9c37473</p>
            </div>
            <div>
              <p>1 day ago</p>
            </div>
            <div class="flexDisplayWrap">
              <div><img class='img flexDisplayWrap' src="../assets/star.png"></div>
              <div>5</div>
              <p>commits</p>
            </div>
          </div>
        </div>
        <div class="tableBody">
          <div class="tableLine flexDisplayWrap">
            <div class="tableFirstLine flexDisplayWrap"><img class='img' src="../assets/star.png"><p>file name</p></div>
            <div><p>commit name</p></div>
            <div><p>commit date</p></div>
          </div>
          <div class="tableLine flexDisplayWrap">
            <div class="tableFirstLine flexDisplayWrap"><img class='img' src="../assets/star.png"><p>file name</p></div>
            <div><p>commit name</p></div>
            <div><p>commit date</p></div>
          </div>
        </div>
      </div>
      <div class="readMe">
        <div class="readMeName flexDisplayWrap">
          <p>README.md</p>
          <div><img class='img' src="../assets/star.png"></div>
        </div>
        <div class="readMeContent">
          <p>GitHub clone by guic97</p>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name:"siteSection",
}
</script>

<style scoped>
  .main{
    max-width: 1000px;
    align-items: center;
    justify-content: flex-start;
    color: white;
  }
  .flexDisplayWrap{
    align-items: center;
  }
  section{
    padding: 30px 10px;
    width: 900px;
  }
  .leftButtons div, .rightButtons div{
    display: flex;
    flex-wrap: wrap;
    margin-right: 8px;
  }
  .topButtons, .topButtons div, .repositoryName{
    justify-content: space-between;
  }
  .button{
    background-color: rgb(38, 38, 53);
    padding: 6px 15px;
    border-radius: 8px;
    color: blanchedalmond;
    border: 1px solid #444;
    font-weight: bold;
  }
  .button:hover{
    background-color: rgb(56, 56, 77);
    border-color: #888;
  }
  #codeButton{
    background-color: rgba(0, 255, 13, 0.678);
    padding: 5px 20px;
  }
  #codeButton:hover{
    background-color: rgba(0, 255, 13, 0.733);
  }
  .buttonTwo{
    margin: 0px;
    padding: auto;
    justify-items: center;
    align-content: center;
  }
  .buttonTwo h3{
    margin-left: 5px;
  }
  .buttonTwo:hover{
    color: rgb(0, 153, 255);
  }
  a img{
    width: 25px;
    border: 1px solid #555;
    border-radius: 30px;
  }
  .repository, .readMe{
    background-color: rgb(16, 19, 24);
    border: 1px solid #333;
    margin: 15px 0;
    border-radius: 5px;
  }
  .repositoryName{
    border-radius: 5px;
    padding: 15px 0;
    background-color: rgba(38, 38, 53, 0.383);
  }
  .leftContent{
    margin-left: 12px;
    align-items:center;
  }
  .leftContent a{
    text-decoration: none;
    color:rgba(255, 255, 255, 0.856);
  }
  .leftContent a:hover, .rightContent p:hover, .tableLine div:hover{
    cursor: pointer;
    color: rgb(0, 153, 255);
    text-decoration: underline;
  }
  .rightContent{
    margin-right: 12px;
  }
  .rightContent p, .buttonTwo p{
    color: rgba(255, 255, 255, 0.479);
  }
  .leftContent div, .rightContent div{
    margin-right: 5px;
  }
  .photoDiv{
    margin-top: 4px;
  }
  .tableLine{
    justify-content: space-between;
    border-bottom: 1px solid #333;
    padding: 8px 0;
  }
  .tableLine div{
    margin: 0 20px;
  }
  .tableLine:hover{
    background-color: rgb(33, 31, 43);
  }
  .tableFirstLine p{
    margin-left: 20px;
  }
  .readMeName{
    justify-content: space-between;
    border-radius: 5px;
    padding: 15px;
    font-weight: bold;
    color: rgba(240, 255, 255, 0.637);
  }
  .readMeContent{
    padding: 30px;
  }
  .readMeContent p{
    font-size: 30px;
  }
</style>