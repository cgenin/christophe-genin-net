<template>
   <q-card inline class="bigger bg-white">
      <q-card-media>
        <img src="~assets/donuts.png">
      </q-card-media>
      <q-card-title>
        Cafe Basilico
        <q-rating slot="subtitle" v-model="stars" :max="5" />
        <div slot="right" class="row items-center">
          <q-icon name="place" /> 250 ft
        </div>
      </q-card-title>
      <q-card-main>
        <p>$・Italian, Cafe</p>
        <p class="text-faded">Small plates, salads & sandwiches in an intimate setting.</p>
      </q-card-main>
      <q-card-separator />
      <q-card-actions>
        <q-btn flat round small><q-icon name="event" /></q-btn>
        <q-btn flat>5:30PM</q-btn>
        <q-btn flat>7:30PM</q-btn>
        <q-btn flat>9:00PM</q-btn>
        <q-btn flat color="primary">Reserve</q-btn>
      </q-card-actions>
    </q-card>
</template>
<script>
import { 
  QCard,
  QCardTitle,
  QCardMedia,
  QCardActions,
  QCardSeparator,
  QCardMain,
  QList,
  QItem,
  QItemMain,
  QItemSide,
  QItemTile,
  QCollapsible,
  QRating,
  QBtn,
  QParallax,
  QIcon,
  QPopover,
  QVideo
  } from 'quasar';

export default {
    name: 'CardProject',
    components: {
        QCard,
        QCardTitle,
        QCardMedia,
        QCardActions,
        QCardSeparator,
        QCardMain,
        QList,
        QItem,
        QItemMain,
        QItemSide,
        QItemTile,
        QCollapsible,
        QRating,
        QBtn,
        QParallax,
        QIcon,
        QPopover,
        QVideo
    }
}
</script>
