<template>
<div class="body">
  <div>
    <site-header/>
  </div>

  <div>
    <site-nav/>
  </div>

  <div class="sections flexDisplayWrap">
    <section>
      <site-section/>
    </section>

    <aside>
      <site-aside/>
    </aside>
  </div>

  <footer>
    <site-footer/>
  </footer>
</div>
</template>

<script>
import siteHeader from "./components/siteHeader.vue";
import siteNav from "./components/siteNav.vue";
import siteFooter from "./components/siteFooter.vue";
import siteAside from "./components/siteAside.vue";
import siteSection from "./components/siteSection.vue"
export default {
  name: 'App',
  components: {
   siteHeader,
   siteNav,
   siteFooter,
   siteAside,
   siteSection,
  }
}
</script>

<style>
  *{
    margin: 0px;
    padding: 0px;
    list-style: none;
    font-family: -apple-system,BlinkMacSystemFont,"Segoe UI",Helvetica,Arial,sans-serif,"Apple Color Emoji","Segoe UI Emoji";
    font-size: 14px;
    color: white;
  }
  .flexDisplayWrap{
    display: flex;
    flex-wrap: wrap;
  }
  body{
    background-color: rgb(16, 19, 24);
  }
  .sections{
    margin-left: 25px;
    justify-content: space-around;
  }
  .img{
    width: 15px;
    height: 15px;
    border: 1px solid rgb(229, 255, 0);
  }
</style>
