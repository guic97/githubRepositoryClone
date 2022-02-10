<template>
<div class="body">
  <div>
    <navegation/>
  </div>

  <div>
    <sub-navbar/>
  </div>

  <section>
    <div>

    </div>
  </section>

  <aside>
    <div>

    </div>
  </aside>

  <footer>
    <div>

    </div>
  </footer>
</div>
</template>

<script>
import navegation from "./components/navegation.vue";
import subNavbar from "./components/subNavbar.vue";
export default {
  name: 'App',
  components: {
   navegation,
   subNavbar,
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
  body{
    background-color: rgb(16, 19, 24);
  }
  
</style>
