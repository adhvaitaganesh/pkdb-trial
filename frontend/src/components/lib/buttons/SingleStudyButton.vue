<template>
  <v-btn color="black"
         text
         width="100%"
         title="Show example dataset"
         to="/data/PKDB00057/"
  >
    <v-icon left color="#1E90FF">{{ faIcon('data') }}</v-icon>
    {{text}}
  </v-btn>
</template>

<script>
import {IconsMixin} from "../../../icons";

export default {
  name: "SingleStudyButton",
  mixins: [IconsMixin],
  props: {
    text: {
      type:String,
      default:"Example dataset"
    },
  }

}
</script>

<style scoped>

</style>
