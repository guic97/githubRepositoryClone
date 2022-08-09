<template>
  <!--

    npm install -g @vue/cli ( instalar vue )
    npm install ( instalar o node_modules )
    npm run serve ( iniciar o vue )

  -->
  <main class="body">
    <div class="header">
      <header>
        <site-header/>
      </header>
      <nav>
        <site-nav/>
      </nav>
    </div>

    <div class=" sections">
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

  </main>
</template>

<script>
import siteHeader from "./components/siteHeader.vue";
import siteNav from "./components/siteNav.vue";
import siteFooter from "./components/siteFooter.vue";
import siteAside from "./components/siteAside.vue";
import siteSection from "./components/siteSection.vue";

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
  }
  .flexDisplayWrap{
    display: flex;
    flex-wrap: wrap;
  }
  main{
    background-color: rgb(16, 19, 24);
  }
  .sections{
    display: flex;
    flex-direction: row;
    margin: auto;
    padding: 0 32px;
    padding-bottom: 32px;
  }
  .img{
    width: 15px;
    height: 15px;
    border: 1px solid rgb(0, 0, 0);
    background-color: #666;
  }
  @media screen and (max-width: 768px) {
    aside{
      display: none;
    }
  }
</style>
