<template>
 

    <!--
      Replace following <div> with
      <router-view /> component
      if using subRoutes
    -->
    <div class="main absolute-top absolute-bottom">
      <div class="presentation bg-white row  main shadow-2">
      <img src="https://avatars3.githubusercontent.com/u/8105661?s=460&v=4">
        <div class="column">
          <h3>Christophe Genin</h3>
          <p>I am an full stack developper with more 15 years of experiences. Based in region of Niort in France.</p>
          <p>My technologie's interests are : Java stacks (J2EE, Spring, Vertx, etc...), Javascript, React, Vue.js, nodejs and plenty other's cool things.</p>
          <div class="row justify-around wrap">   
            <q-btn @click="launch('https://github.com/cgenin')" round icon="fa-github" color="secondary"></q-btn> 
            <q-btn @click="launch('https://twitter.com/skarboune')" round icon="fa-twitter" color="secondary"></q-btn> 
          </div>
        </div>
      </div>
    </div>
 
</template>

<script>
import {
  QCard, QBtn, openURL
} from 'quasar'

export default {
  name: 'about',
  components: {
    QCard, QBtn
  }, 
  methods: {
    launch(url) {
      openURL(url);
    }
  }
}
</script>

<style scoped>
.main {
  display: flex;
  justify-content: center;
  align-items: center;

}
.presentation {
  margin: auto;
  padding: 10px;
}
</style>
