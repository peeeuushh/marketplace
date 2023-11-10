<template>
<div>

     <q-card>
      <q-card-title style="font-size: x-large;align-items: center;"> Search Results </q-card-title> </q-card><br>
  <div class="q-pa-md row items-start q-gutter-md" v-for="index in 10" :key="index" >

       <div >

    <q-card class="my-card" clickable @click= "MainLayout">

        <q-card-section>
        <q-btn
          fab
          style="top: 20px;bottom:70px ; right: 12px; transform: translateY(-50%);"
        />
        <div class="row no-wrap items-center"></div>
          <div class="col text-h6 ellipsis">
          APP 1
          </div>
          <div class="col text-h6 ellipsis">
          Public
          </div>
          <q-rating v-model="stars" :max="5" size="32px" />
        </q-card-section>
        <q-card-section class="q-pt-none">
        <div class="text-subtitle1">
          1M+ Downloads
        </div>
        <div class="text-caption text-black">
         this is the app description.
        </div>
      </q-card-section>

      <q-separator />


    </q-card><br>
  </div>

    <q-card class="my-card">
      <q-card-section>
        <q-btn
          fab
          style="top: 20px;bottom:70px ; right: 12px; transform: translateY(-50%);"
        />
        <div class="row no-wrap items-center"/>
          <div class="col text-h6 ellipsis">
          APP 2
          </div>
          <div class="col text-h6 ellipsis">
          Public
          </div>
          <q-rating v-model="stars" :max="5" size="32px" />
        </q-card-section>
        <q-card-section class="q-pt-none">
        <div class="text-subtitle1">
          1M+ Downloads
        </div>
        <div class="text-caption text-black">
         this is the app2 description.
        </div>
      </q-card-section>
      <q-separator />


    </q-card><br>
    <q-card class="my-card">
      <q-card-section>
        <q-btn
          fab
          style="top: 20px;bottom:70px ; right: 12px; transform: translateY(-50%);"
        />
        <div class="row no-wrap items-center"/>
          <div class="col text-h6 ellipsis">
          APP 3
          </div>
          <div class="col text-h6 ellipsis">
          Public
          </div>
          <q-rating v-model="stars" :max="5" size="32px" />
        </q-card-section>
        <q-card-section class="q-pt-none">
        <div class="text-subtitle1">
          1M+ Downloads
        </div>
        <div class="text-caption text-black">
         this is the app3 description.
        </div>
      </q-card-section>
      <q-separator />


    </q-card>
  </div>
<!-- </q-col>
  </q-row> -->

</div>
</template>
<script>
import MainLayout from 'src/layouts/MainLayout.vue';
import IndexPage from 'src/pages/IndexPage.vue';
import { ref } from 'vue'

export default {
  setup () {
    return {
      stars: ref(4),
      cards:[1,2]
    }
  }
}
</script>
<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 300px
// .card-container
// {
//   display: grid;
//   grid-template-columns: repeat(2,1fr);
//   gap: 16px;
// }
</style>
