<template>
  <v-layout wrap align-center justify-center>
    <v-flex text-center xs12>
      <div class="title-text">Slider</div>
      <link-buttons
        document="https://vuetifyjs.com/en/components/sliders"
        source="https://github.com/reireias/vuetifier/blob/master/components/SliderSample.vue"
      ></link-buttons>
    </v-flex>
    <v-flex text-center xs12>
      <v-slider
        value="50"
        label="Normal"
        :dark="$vuetify.theme.dark"
      ></v-slider>
    </v-flex>
    <v-flex text-center xs12>
      <v-slider
        value="50"
        color="secondary"
        prepend-icon="volume_down"
        append-icon="volume_up"
        :dark="$vuetify.theme.dark"
      ></v-slider>
    </v-flex>
    <v-flex text-center xs12>
      <v-range-slider
        :value="[30, 60]"
        color="accent"
        label="Range"
      ></v-range-slider>
    </v-flex>
  </v-layout>
</template>

<script>
import LinkButtons from '@/components/LinkButtons'
export default {
  components: {
    LinkButtons,
  },
}
</script>
