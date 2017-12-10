<template>
  <!-- Don't drop "q-app" class -->
  <div id="q-app">
     <q-layout
    ref="layout"
    view="lHh Lpr fff"
    :left-class="{'bg-primary': true, 'text-white':true}"
  >
    <q-toolbar slot="header">
      <q-btn
        flat
        @click="$refs.layout.toggleLeft()"
      >
        <q-icon name="menu" />
      </q-btn>

      <q-toolbar-title>
         Christophe-genin.net
        <div slot="subtitle">An developper's site</div>
      </q-toolbar-title>
    </q-toolbar>

    <div  class=" " slot="left">
      <!--
        Use <q-side-link> component
        instead of <q-item> for
        internal vue-router navigation
      -->

      <q-list no-border link inset-delimiter>
        <q-list-header class="text-white">Site plan</q-list-header>
        <q-item to="/projects">
          <q-item-side color="white" icon="school" />
          <q-item-main label="Open Source projects" sublabel="My github's projects" />
        </q-item>
        <q-item to="/about">
          <q-item-side  color="white"  icon="account_box" />
          <q-item-main label="About me" sublabel="Christophe Genin" />
        </q-item>
      
      </q-list>
    </div>
    <router-view />
     </q-layout>
  </div>
</template>

<script>
import {
  QLayout,
  QToolbar,
  QToolbarTitle,
  QBtn,
  QIcon,
  QList,
  QListHeader,
  QItem,
  QItemSide,
  QItemMain
} from 'quasar'
/*
 * Root component
 */
export default {
  components: {
    QLayout,
    QToolbar,
    QToolbarTitle,
    QBtn,
    QIcon,
    QList,
    QListHeader,
    QItem,
    QItemSide,
    QItemMain
  }
}
</script>

<style>

.q-item-sublabel{
  color:#dddbdb;
}
</style>
