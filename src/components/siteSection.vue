<template>
  <div class="main flexDisplayWrap">
    <section class="section">
      <div class="topButtons flexDisplayWrap">
        <div class="leftButtons flexDisplayWrap">
            <div>
                <div><img class='img' src="../assets/star.png"></div>
                <div><p>master</p></div>
            </div>
            <div>
                <div><img class='img' src="../assets/star.png"></div>
                <div><p>1 branch</p></div>
            </div>
            <div>
                <div><img class='img' src="../assets/star.png"></div>
                <div><p>0 tags</p></div>
            </div>
        </div>
        <div class="rightButtons flexDisplayWrap">
            <div class="button">
                <img class="img" src="../assets/star.png" >
                <p>Go to file</p>
            </div>
            <div class="button">
                <img class="img" src="../assets/star.png" >
                <p>Add file</p>
            </div>
            <div class="button">
                <img class="img" src="../assets/star.png" >
                <p>Code</p>
            </div>
        </div>
      </div>
      <div class="repository">
        <div class="repositoryName">
          <div class="leftContent">
            <div></div>
          </div>
          <div class="rightContent">
            <div>
                <p>9c37473</p>
            </div>
            <div>
                <p>1 day ago</p>
            </div>
            <div>
              <div><img class='img' src="../assets/star.png"></div>
              <div><p>6 commits</p></div>
            </div>
          </div>
        </div>
        <div>
          <p>Imagine a table here</p>
        </div>
      </div>
      <div class="readMe">
        <div class="readMeName">
          <p>Name.md</p>
        </div>
        <div class="readMeContent">
          <p>Something here</p>
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
    background-color: blue;
    align-items: center;
    justify-content: flex-start;
  }
  section{
    padding: 30px 20px;
    width: 900px;
  }
  .leftButtons div, .rightButtons div{
    display: flex;
    flex-wrap: wrap;
  }
  .topButtons{
    justify-content: space-between;
  }
  .topButtons div{
    justify-content: space-between;
  }
</style>