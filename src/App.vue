<template>
<div class="body">
  <div>
    <site-header/>
  </div>

  <div>
    <sub-navbar/>
  </div>

  <section>
    <div>

    </div>
  </section>

  <aside>
    <site-aside/>
  </aside>

  <footer>
    <site-footer/>
  </footer>
</div>
</template>

<script>
import siteHeader from "./components/siteHeader.vue";
import subNavbar from "./components/subNavbar.vue";
import siteFooter from "./components/siteFooter.vue";
import siteAside from "./components/siteAside.vue";

export default {
  name: 'App',
  components: {
   siteHeader,
   subNavbar,
   siteFooter,
   siteAside,
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
  
</style>
