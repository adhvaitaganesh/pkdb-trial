<template>
  <v-main class="trial">
    <v-container>
      <v-row class="page-hero" align="center">
        <v-col cols="12" md="7">
          <p class="eyebrow">Dataset ingestion</p>
          <h1 class="hero-title">Upload, validate, and package lab datasets.</h1>
          <p class="lead">
            Centralize assays, protocols, and raw files into a single submission pipeline with automated checks and
            provenance metadata.
          </p>
        </v-col>
        <v-col cols="12" md="5">
          <v-card outlined class="hero-card">
            <v-card-title class="subtitle-1 font-weight-bold">Active submission</v-card-title>
            <v-divider></v-divider>
            <v-list dense>
              <v-list-item>
                <v-list-item-content>
                  <v-list-item-title class="font-weight-bold">PK Liver Panel v3</v-list-item-title>
                  <v-list-item-subtitle>Owner: A. Singh · 64 files</v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content>
                  <v-list-item-title class="font-weight-bold">Validation status</v-list-item-title>
                  <v-list-item-subtitle>3 warnings · 1 required fix</v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
            </v-list>
            <v-card-subtitle>Last updated 15 minutes ago</v-card-subtitle>
          </v-card>
        </v-col>
      </v-row>

      <section class="section">
        <div class="section-heading">
          <h2>Upload workspace</h2>
          <p>Drag and drop files or connect an instrument export to start a submission.</p>
        </div>
        <v-row>
          <v-col cols="12" md="6">
            <v-card outlined class="tile">
              <h3>Drop files</h3>
              <p>Supports CSV, XLSX, FASTQ, and assay exports. Max 25 GB per upload.</p>
              <div class="upload-drop">
                <div>
                  <strong>Drop files here</strong>
                  <div class="muted">or browse from your device</div>
                </div>
                <v-btn outlined color="primary">Browse files</v-btn>
              </div>
            </v-card>
          </v-col>
          <v-col cols="12" md="6">
            <v-card outlined class="tile">
              <h3>Submission checklist</h3>
              <v-list dense class="checklist">
                <v-list-item>
                  <v-chip small color="green" text-color="white" class="mr-2">Done</v-chip>
                  <span>Study metadata captured</span>
                </v-list-item>
                <v-list-item>
                  <v-chip small color="amber darken-2" text-color="white" class="mr-2">Needs review</v-chip>
                  <span>Instrument calibration report</span>
                </v-list-item>
                <v-list-item>
                  <v-chip small color="grey lighten-1" text-color="white" class="mr-2">Pending</v-chip>
                  <span>Protocol attachments</span>
                </v-list-item>
                <v-list-item>
                  <v-chip small color="grey lighten-1" text-color="white" class="mr-2">Pending</v-chip>
                  <span>Data steward approval</span>
                </v-list-item>
              </v-list>
            </v-card>
          </v-col>
        </v-row>
      </section>

      <section class="section muted">
        <div class="section-heading">
          <h2>Validation & enrichment</h2>
          <p>Resolve automated checks and add structured metadata before publishing.</p>
        </div>
        <v-row>
          <v-col cols="12" md="4">
            <v-card outlined class="tile">
              <h3>Schema validation</h3>
              <p>Run column mapping, unit normalization, and controlled vocabulary checks.</p>
            </v-card>
          </v-col>
          <v-col cols="12" md="4">
            <v-card outlined class="tile">
              <h3>Sample mapping</h3>
              <p>Link specimen IDs, cohorts, and treatment arms to each assay file.</p>
            </v-card>
          </v-col>
          <v-col cols="12" md="4">
            <v-card outlined class="tile">
              <h3>Quality gates</h3>
              <p>Configure pass/fail thresholds and required documentation per study type.</p>
            </v-card>
          </v-col>
        </v-row>
      </section>
    </v-container>
  </v-main>
</template>

<script>
export default {
  name: 'TrialUpload',
}
</script>

<style scoped>
.trial {
  background: #fff;
}

.page-hero {
  margin-top: 24px;
}

.hero-title {
  font-size: clamp(2rem, 4vw, 3rem);
  line-height: 1.1;
  margin-bottom: 16px;
}

.eyebrow {
  text-transform: uppercase;
  font-weight: 600;
  letter-spacing: 0.15em;
  font-size: 0.75rem;
  color: #3d57ff;
  margin-bottom: 12px;
}

.lead {
  color: #475569;
  margin-bottom: 24px;
}

.hero-card {
  background: #f8fafc;
}

.section {
  margin-top: 48px;
}

.section.muted {
  background: #f8fafc;
  padding: 32px;
  border-radius: 20px;
}

.section-heading p {
  color: #475569;
  max-width: 720px;
}

.tile {
  padding: 20px;
}

.tile p,
.muted {
  color: #475569;
}

.upload-drop {
  margin-top: 16px;
  border: 1px dashed #e2e8f0;
  border-radius: 16px;
  padding: 16px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 16px;
  background: #f8fafc;
}

.checklist {
  padding: 0;
}

.checklist .v-list-item {
  padding-left: 0;
}
</style>
