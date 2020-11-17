<template>
  <div id="app">
    <header>
      <Navbar />
    </header>
    <main>
      <IntroduceBlock />
      <ArticleBlock />
    </main>
    <footer>
      <Information />
    </footer>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import IntroduceBlock from './components/IntroduceBlock.vue';
import ArticleBlock from './components/ArticleBlock.vue';
import Information from './components/Information.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    IntroduceBlock,
    ArticleBlock,
    Information
  }
}
</script>

<style>
body {
  padding: 0;
  margin: 0;
}

header {
  background-color: #eeeeee;
  border-bottom: 1px solid #EAEAEA;
  padding: 30px 0 45px;
  text-align: center;
}

footer {
  background-color: #eeeeee;
  border-top: 1px solid #EAEAEA;
  padding: 32px 0 20px;
}

</style>
