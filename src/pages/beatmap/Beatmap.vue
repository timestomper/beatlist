<template>
  <v-container>
    <transition name="slide-x-transition" mode="out-in">
      <keep-alive>
        <router-view :key="$route.path" />
      </keep-alive>
    </transition>
  </v-container>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "Beatmap",
});
</script>
