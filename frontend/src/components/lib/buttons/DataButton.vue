<template>
  <v-btn color="black"
         text
         width="100%"
         to="/data"
         title="Browse data catalog"
  >
    <v-icon left color="#1E90FF">{{ faIcon('data') }}</v-icon>
    Browse catalog
  </v-btn>
</template>

<script>
import {IconsMixin} from "../../../icons";

export default {
  name: "DataButton",
  mixins: [IconsMixin]

}
</script>

<style scoped>

</style>
