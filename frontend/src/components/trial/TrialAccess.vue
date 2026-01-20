<template>
  <v-main class="trial">
    <v-container>
      <v-row class="page-hero" align="center">
        <v-col cols="12" md="7">
          <p class="eyebrow">Governance</p>
          <h1 class="hero-title">Define access tiers and data-use agreements.</h1>
          <p class="lead">
            Control who can view, download, and publish datasets with role-based permissions, embargo windows, and
            approval workflows.
          </p>
        </v-col>
        <v-col cols="12" md="5">
          <v-card outlined class="hero-card">
            <v-card-title class="subtitle-1 font-weight-bold">Access overview</v-card-title>
            <v-divider></v-divider>
            <v-list dense>
              <v-list-item>
                <v-list-item-content>
                  <v-list-item-title class="font-weight-bold">24 active collaborators</v-list-item-title>
                  <v-list-item-subtitle>Across 6 partner organizations</v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content>
                  <v-list-item-title class="font-weight-bold">5 pending requests</v-list-item-title>
                  <v-list-item-subtitle>Awaiting governance review</v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
            </v-list>
            <v-card-subtitle>Policy updates synced today</v-card-subtitle>
          </v-card>
        </v-col>
      </v-row>

      <section class="section">
        <div class="section-heading">
          <h2>Permission tiers</h2>
          <p>Assign each dataset a visibility tier that maps to roles, export formats, and agreements.</p>
        </div>
        <v-row>
          <v-col cols="12" md="4">
            <v-card outlined class="tile">
              <h3>Internal research</h3>
              <p>Full dataset access for lab teams and modeling groups with internal SOP compliance.</p>
              <ul class="meta-list">
                <li>Download raw files</li>
                <li>Export analysis-ready tables</li>
                <li>Attach internal notes</li>
              </ul>
            </v-card>
          </v-col>
          <v-col cols="12" md="4">
            <v-card outlined class="tile">
              <h3>External partner</h3>
              <p>Restricted views with watermarking, curated subsets, and required acknowledgements.</p>
              <ul class="meta-list">
                <li>Read-only access</li>
                <li>Data-use agreement required</li>
                <li>24-hour audit log</li>
              </ul>
            </v-card>
          </v-col>
          <v-col cols="12" md="4">
            <v-card outlined class="tile">
              <h3>Public release</h3>
              <p>Publish vetted datasets with citations and open access metadata.</p>
              <ul class="meta-list">
                <li>Landing page + DOI</li>
                <li>Dataset versioning</li>
                <li>Community visibility</li>
              </ul>
            </v-card>
          </v-col>
        </v-row>
      </section>

      <section class="section muted">
        <div class="section-heading">
          <h2>Approval workflow</h2>
          <p>Route requests and approvals through governance checkpoints.</p>
        </div>
        <v-row>
          <v-col cols="12" md="6">
            <v-card outlined class="tile">
              <h3>Request queue</h3>
              <div class="queue-item">
                <div>
                  <strong>Genomic Safety Signals</strong>
                  <div class="muted">Requested by Horizon Bio · 2 days ago</div>
                </div>
                <v-btn outlined color="primary">Review request</v-btn>
              </div>
              <div class="queue-item">
                <div>
                  <strong>PK Liver Panel v3</strong>
                  <div class="muted">Requested by MedCore Labs · 4 days ago</div>
                </div>
                <v-btn outlined color="primary">Review request</v-btn>
              </div>
            </v-card>
          </v-col>
          <v-col cols="12" md="6">
            <v-card outlined class="tile">
              <h3>Usage agreements</h3>
              <p>Attach agreements and expiration dates to every share, and capture signatures.</p>
              <div class="queue-item">
                <div>
                  <strong>Standard pharma NDA</strong>
                  <div class="muted">Expires Dec 2025 · 18 active datasets</div>
                </div>
                <v-btn text color="primary">View template</v-btn>
              </div>
              <div class="queue-item">
                <div>
                  <strong>AI research license</strong>
                  <div class="muted">Expires May 2026 · 9 active datasets</div>
                </div>
                <v-btn text color="primary">View template</v-btn>
              </div>
            </v-card>
          </v-col>
        </v-row>
      </section>
    </v-container>
  </v-main>
</template>

<script>
export default {
  name: 'TrialAccess',
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

.meta-list {
  padding-left: 18px;
  color: #475569;
}

.queue-item {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 12px;
  padding-top: 16px;
  margin-top: 16px;
  border-top: 1px solid #e2e8f0;
}

.queue-item:first-of-type {
  border-top: none;
  padding-top: 0;
  margin-top: 0;
}
</style>
