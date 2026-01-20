<template>
  <div>
  <h2>Sample dataset preview</h2>

    <p align="justify">
      Preview how a curated dataset captures assay context, cohort metadata, and key outputs.
    </p>

    <p>
      <curation-example-image/>
    </p>

    <p>
      <single-study-button text="View sample dataset"/>

  </p>
  </div>
</template>

<script>
import SingleStudyButton from "../lib/buttons/SingleStudyButton";

import {IconsMixin} from "@/icons";
import CurationExampleImage from "./CurationExampleImage";
export default {
  name: "CurationExample",
  mixins: [IconsMixin],
  components:{CurationExampleImage, SingleStudyButton}
}
</script>
