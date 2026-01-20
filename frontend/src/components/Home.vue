<template>
  <v-main id="home" class="pl-1 pr-1">
    <v-container fluid>
      <v-row align="start"
             justify="center">
        <v-col xs="11" sm="11" md="10" lg="8">
          <section>
            <h1>Pharma Data Exchange</h1>
            <p align="justify">
              A shared workspace where pharma scientists upload and curate laboratory datasets, while AI researchers
              discover approved data through powerful filters and clear provenance.
            </p>
            <v-sheet class="mt-4 pa-4" outlined>
              <v-row>
                <v-col cols="12" md="4">
                  <strong>Upload & organize</strong>
                  <p class="mb-0">Capture studies, cohorts, and assay context in a single place.</p>
                </v-col>
                <v-col cols="12" md="4">
                  <strong>Control access</strong>
                  <p class="mb-0">Define who can view, request, or download each dataset.</p>
                </v-col>
                <v-col cols="12" md="4">
                  <strong>Publish to AI teams</strong>
                  <p class="mb-0">Share curated releases with data-ready metadata.</p>
                </v-col>
              </v-row>
            </v-sheet>
          </section>

          <section class="mt-6">
            <h2>Built for two audiences</h2>
            <v-row>
              <v-col cols="12" md="6">
                <v-card outlined class="pa-4">
                  <h3>Pharma scientists & lab teams</h3>
                  <ul>
                    <li>Upload raw files, structured tables, and protocols.</li>
                    <li>Group datasets by study, cohort, and experiment.</li>
                    <li>Publish approved releases with access rules.</li>
                  </ul>
                </v-card>
              </v-col>
              <v-col cols="12" md="6">
                <v-card outlined class="pa-4">
                  <h3>AI researchers & data partners</h3>
                  <ul>
                    <li>Search by assay, compound, cohort, or output.</li>
                    <li>Review dataset cards with provenance details.</li>
                    <li>Request access or download approved datasets.</li>
                  </ul>
                </v-card>
              </v-col>
            </v-row>
          </section>

          <section class="mt-6">
            <h2>From upload to publication</h2>
            <v-row>
              <v-col cols="12" md="4">
                <v-card outlined class="pa-4">
                  <h3>1. Ingest</h3>
                  <p>Drop files, validate metadata, and capture experiment context.</p>
                </v-card>
              </v-col>
              <v-col cols="12" md="4">
                <v-card outlined class="pa-4">
                  <h3>2. Curate</h3>
                  <p>Standardize fields, add ontologies, and link assays to cohorts.</p>
                </v-card>
              </v-col>
              <v-col cols="12" md="4">
                <v-card outlined class="pa-4">
                  <h3>3. Share</h3>
                  <p>Publish controlled releases and track who can access each dataset.</p>
                </v-card>
              </v-col>
            </v-row>
          </section>

          <section class="mt-6">
            <h2>Browse the catalog</h2>
            <p align="justify">
              Explore the live dataset inventory to see the range of studies, cohorts, and outputs already available.
            </p>
            <data-button/>
            <p>
              <count-table/>
            </p>
          </section>

          <section class="mt-6">
            <curation-example />
          </section>

          <about />
        </v-col>
      </v-row>
    </v-container>
  </v-main>
</template>

<script>
import CurationExample from "./home/CurationExample";
import CountTable from "./tables/CountTable";
import About from './home/About';
import {IconsMixin} from "@/icons";
import DataButton from "./lib/buttons/DataButton";

export default {
  name: "Home",
  components: {
    DataButton,
    // StatisticsVegaPlot,
    CountTable,
    CurationExample,
    About
  },
  mixins: [IconsMixin],
}
</script>

<style>
</style>
