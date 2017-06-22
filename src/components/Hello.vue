<template>
  <div class="demo-layout-waterfall mdl-layout mdl-js-layout">
    <header class="mdl-layout__header mdl-layout__header--waterfall">
      <!-- Top row, always visible -->
      <div class="mdl-layout__header-row">
        <!-- Title -->
        <span class="mdl-layout-title">Title</span>
        <!--<div class="mdl-layout-spacer"></div>-->
        <!--<div class="mdl-textfield mdl-js-textfield mdl-textfield--expandable
                        mdl-textfield--floating-label mdl-textfield--align-right">
          <label class="mdl-button mdl-js-button mdl-button--icon"
                 for="waterfall-exp">
            <i class="material-icons">search</i>
          </label>
          <div class="mdl-textfield__expandable-holder">
            <input class="mdl-textfield__input"
                   type="text"
                   name="sample"
                   id="waterfall-exp">
          </div>
        </div>-->
      </div>
      <!-- Bottom row, not visible on scroll -->
      <div class="mdl-layout__header-row">
        <div class="mdl-layout-spacer"></div>
        <!-- Navigation -->
        <nav class="mdl-navigation">
          <a class="mdl-navigation__link"
             href="">Link1</a>
          <a class="mdl-navigation__link"
             href="">Link2</a>
          <a class="mdl-navigation__link"
             href="">Link3</a>
          <a class="mdl-navigation__link"
             href="">Link4</a>
        </nav>
      </div>
    </header>
    <div class="mdl-layout__drawer">
      <span class="mdl-layout-title">Title</span>
      <nav class="mdl-navigation">
        <a class="mdl-navigation__link"
           href="">Link1</a>
        <a class="mdl-navigation__link"
           href="">Link2</a>
        <a class="mdl-navigation__link"
           href="">Link3</a>
        <a class="mdl-navigation__link"
           href="">Link4</a>
      </nav>
    </div>
    <main class="mdl-layout__content">
      <div class="page-content">
        <!-- Your content goes here -->
        <contents></contents>
      </div>
    </main>
  </div>
</template>

<script>
import contents from '@/components/Contents'
export default {
  data() {
    return {
      value: 3
    }
  },
  components: {
    contents
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}

.demo-layout-waterfall .mdl-layout__header-row .mdl-navigation__link:last-of-type {
  padding-right: 0;
}
</style>
