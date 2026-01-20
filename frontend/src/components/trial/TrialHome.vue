<template>
  <v-main class="trial">
    <v-container>
      <v-row class="hero" align="center">
        <v-col cols="12" md="7">
          <p class="eyebrow">Pharma data exchange</p>
          <h1 class="hero-title">Organize, publish, and discover research datasets with confidence.</h1>
          <p class="lead">
            Trial is a secure workspace for pharma scientists and lab teams to upload studies, apply governance, and share
            curated datasets with internal and external collaborators.
          </p>
          <div class="hero-actions">
            <v-btn color="primary" class="mr-2" to="/trial/upload">Start a trial workspace</v-btn>
            <v-btn outlined color="primary" to="/trial/access">Review access policies</v-btn>
          </div>
          <div class="hero-meta">
            <v-chip small class="mr-2" color="primary" outlined>Audit-ready submissions</v-chip>
            <v-chip small class="mr-2" color="primary" outlined>Granular access control</v-chip>
            <v-chip small color="primary" outlined>AI-ready metadata</v-chip>
          </div>
        </v-col>
        <v-col cols="12" md="5">
          <v-card class="hero-card" outlined>
            <v-card-title class="subtitle-1 font-weight-bold">Today in the lab</v-card-title>
            <v-divider></v-divider>
            <v-list dense>
              <v-list-item>
                <v-list-item-content>
                  <v-list-item-title class="font-weight-bold">12 new datasets</v-list-item-title>
                  <v-list-item-subtitle>uploaded by clinical pharmacology</v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content>
                  <v-list-item-title class="font-weight-bold">8 pending reviews</v-list-item-title>
                  <v-list-item-subtitle>awaiting data stewardship</v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content>
                  <v-list-item-title class="font-weight-bold">4 shared releases</v-list-item-title>
                  <v-list-item-subtitle>published to external partners</v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
            </v-list>
            <v-card-subtitle>Last synced 2 minutes ago</v-card-subtitle>
          </v-card>
        </v-col>
      </v-row>

      <section class="section">
        <div class="section-heading">
          <h2>Built for regulated research teams.</h2>
          <p>
            Trial turns raw lab outputs into trusted, reusable datasets that comply with internal SOPs and external data
            sharing policies.
          </p>
        </div>
        <v-row>
          <v-col cols="12" md="4">
            <v-card outlined class="tile">
              <h3>Structured submissions</h3>
              <p>Capture assays, protocols, and study metadata with guided templates and automated validation.</p>
            </v-card>
          </v-col>
          <v-col cols="12" md="4">
            <v-card outlined class="tile">
              <h3>Publication-ready releases</h3>
              <p>Package datasets with citations, versioning, and export bundles for collaborators or public release.</p>
            </v-card>
          </v-col>
          <v-col cols="12" md="4">
            <v-card outlined class="tile">
              <h3>Trust & compliance</h3>
              <p>Track lineage, steward approvals, and data usage commitments with every dataset.</p>
            </v-card>
          </v-col>
        </v-row>
      </section>

      <section class="section muted">
        <div class="section-heading">
          <h2>From bench to data repository.</h2>
          <p>Map every step of the lab workflow to an auditable, searchable record.</p>
        </div>
        <v-row>
          <v-col cols="12" md="3">
            <v-card outlined class="tile">
              <span class="step-number">01</span>
              <h3>Upload & validate</h3>
              <p>Drop raw files, capture study context, and resolve validation warnings in one view.</p>
            </v-card>
          </v-col>
          <v-col cols="12" md="3">
            <v-card outlined class="tile">
              <span class="step-number">02</span>
              <h3>Curate & enrich</h3>
              <p>Standardize units, annotate variables, and link to controlled vocabularies.</p>
            </v-card>
          </v-col>
          <v-col cols="12" md="3">
            <v-card outlined class="tile">
              <span class="step-number">03</span>
              <h3>Review & approve</h3>
              <p>Route datasets for stewardship review and capture approval history.</p>
            </v-card>
          </v-col>
          <v-col cols="12" md="3">
            <v-card outlined class="tile">
              <span class="step-number">04</span>
              <h3>Publish & share</h3>
              <p>Release to private collaborators or open catalogs with configurable visibility.</p>
            </v-card>
          </v-col>
        </v-row>
      </section>

      <section class="section">
        <div class="section-heading">
          <h2>Discovery for AI researchers.</h2>
          <p>Search curated datasets using meaningful filters and reusable data descriptors.</p>
        </div>
        <v-row>
          <v-col cols="12" md="6">
            <v-card outlined class="tile">
              <h3>Smart filtering</h3>
              <ul>
                <li>Therapeutic area, molecule, and assay type</li>
                <li>Population, dosing regimen, and sample matrix</li>
                <li>Regulatory status, version, and access tier</li>
              </ul>
            </v-card>
          </v-col>
          <v-col cols="12" md="6">
            <v-card outlined class="tile">
              <h3>Dataset cards</h3>
              <p>
                Preview collection quality with coverage, sample counts, and linked publications before requesting access.
              </p>
              <div class="dataset-row">
                <div>
                  <strong>PK Liver Panel v3</strong>
                  <span>42 cohorts · 1.2M records</span>
                </div>
                <v-btn text small color="primary">View details</v-btn>
              </div>
              <div class="dataset-row">
                <div>
                  <strong>Clinical Safety Signals</strong>
                  <span>14 studies · 28 biomarkers</span>
                </div>
                <v-btn text small color="primary">View details</v-btn>
              </div>
            </v-card>
          </v-col>
        </v-row>
      </section>

      <section class="section muted">
        <div class="section-heading">
          <h2>Access control without bottlenecks.</h2>
          <p>Grant the right people the right access with tiered permissions and traceable agreements.</p>
        </div>
        <v-row>
          <v-col cols="12" md="4">
            <v-card outlined class="tile">
              <h3>Role-based permissions</h3>
              <p>Define lab, stewardship, and collaborator roles down to dataset fields and export formats.</p>
            </v-card>
          </v-col>
          <v-col cols="12" md="4">
            <v-card outlined class="tile">
              <h3>Usage agreements</h3>
              <p>Attach data-use clauses, embargo windows, and attribution requirements to every share.</p>
            </v-card>
          </v-col>
          <v-col cols="12" md="4">
            <v-card outlined class="tile">
              <h3>Secure collaboration</h3>
              <p>Invite external partners with time-bound access and compliance-ready audit trails.</p>
            </v-card>
          </v-col>
        </v-row>
      </section>

      <section class="callout">
        <div>
          <h2>Ready to stand up your data exchange?</h2>
          <p>Launch a Trial workspace and onboard your first dataset in days, not months.</p>
        </div>
        <v-btn color="primary">Schedule a demo</v-btn>
      </section>
    </v-container>
  </v-main>
</template>

<script>
export default {
  name: 'TrialHome',
}
</script>

<style scoped>
.trial {
  background: #fff;
}

.hero {
  margin-top: 24px;
}

.hero-title {
  font-size: clamp(2rem, 4vw, 3.2rem);
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

.hero-actions {
  margin-bottom: 16px;
}

.hero-meta {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
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

.section-heading h2 {
  margin-bottom: 12px;
}

.section-heading p {
  color: #475569;
  max-width: 720px;
}

.tile {
  padding: 20px;
}

.tile p,
.tile li {
  color: #475569;
}

.step-number {
  display: inline-block;
  font-weight: 700;
  color: #3d57ff;
  margin-bottom: 8px;
}

.dataset-row {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 12px;
  padding-top: 12px;
  margin-top: 12px;
  border-top: 1px solid #e2e8f0;
}

.dataset-row span {
  color: #475569;
  font-size: 0.9rem;
}

.callout {
  margin-top: 48px;
  padding: 32px;
  border-radius: 20px;
  background: #0f172a;
  color: #fff;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 16px;
}

.callout p {
  color: #dbeafe;
}
</style>
