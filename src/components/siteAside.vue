<template>
  <div class="main flexDisplayWrap">
      <div class="aside">
        <div class="about">
          <div class="spaceBetween flexDisplayWrap">
            <div><h3>About</h3></div>
            <div class="button"><img class='img' src="../assets/star.png"></div>
          </div>
          <div class="description">
            <p>No description, website, or topics provided.</p>
          </div>
          <div class="asideButtons">
            <div>
              <img class="img" src="../assets/star.png">
              <p>Readme</p>
            </div>
            <div>
              <img class="img" src="../assets/star.png">
              <p>0 stars</p>
            </div>
            <div>
              <img class="img" src="../assets/star.png">
              <p>1 watching</p>
            </div>
            <div>
              <img class="img" src="../assets/star.png">
              <p>0 forks</p>
            </div>
          </div>
        </div>
        <div class='space'></div>
        <div class="releases">
          <h3>Releases</h3>
          <div>
            <p>No releases published</p>
          </div>
          <div><a href="#">Create a new realease</a></div>
        </div>
        <div class='space'></div>
        <div class="packages">
          <h3>Packages</h3>
          <div>
            <p>No packages published</p>
          </div>
          <div><a href="#">Create a new packages</a></div>
        </div>
        <div class='space'></div>
        <div class="languages">
          <h3>Languages</h3>
          <p>No linguages used</p>
        </div>
      </div>
  </div>
</template>

<script>
export default {
  name:"siteAside",
}
</script>

<style scoped>
  .main{
    justify-content:flex-start;
    align-items: center;
    min-width: 310px;
  }
  .spaceBetween{
    justify-content: space-between;
  }
  .aside{
    margin: 5px 10px;
  }
  .about div, .releases p, .packages p, .languages p{
    padding-top:10px;
  }
  .asideButtons div{
    display: flex;
    flex-wrap: wrap;
  }
  .asideButtons p{
    margin-left: 10px;
  }
  div h3{
    font-size: 15px;
    color: rgba(255, 255, 255, 0.671);
  }
  div a{
    text-decoration: none;
    color: rgb(0, 153, 255);
  }
  div a:hover{
    text-decoration: underline;
  }
  .releases h3:hover, .packages h3:hover{
    color: rgb(29, 161, 248);
    cursor: pointer;
  }
  .img:hover, .asideButtons p:hover{
    color: rgb(29, 161, 248);
    cursor: pointer;
  }
  .space{
    border: 1px solid #333;
    margin: 25px 0;
  }
  p{
    color:rgba(255, 255, 255, 0.452);
  }
  .description{
    font-style: italic;
  }
  .description p{
    font-size: 17px;
  }
</style>
