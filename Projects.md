---
layout: page
title: "Highlights of Projects"
permalink: /projects/
---

<style>
/* Simple, theme-friendly project cards */
.projects {
  display: grid;
  grid-template-columns: 1fr;
  gap: 18px;
}
.project-card {
  border: 1px solid rgba(0,0,0,0.08);
  border-radius: 14px;
  padding: 18px;
  background: rgba(0,0,0,0.02);
}
@media (prefers-color-scheme: dark) {
  .project-card { border-color: rgba(255,255,255,0.12); background: rgba(255,255,255,0.03); }
}
.project-title {
  margin: 0 0 8px 0;
  font-weight: 700;
  font-size: 1.1rem;
}

/* Layout: default is single column; two columns only when .has-media is set */
.project-grid {
  display: grid;
  grid-template-columns: 1fr; /* single column by default */
  gap: 16px;
  align-items: start;
}
.project-card.has-media .project-grid {
  grid-template-columns: 1.15fr 0.85fr; /* text left, image right */
}
.project-desc p { margin: 6px 0 10px; }

.project-media img {
  display: block;
  width: 100%;
  height: auto;
  border-radius: 12px;
  border: 1px solid rgba(0,0,0,0.08);
}
@media (prefers-color-scheme: dark) {
  .project-media img { border-color: rgba(255,255,255,0.12); }
}

.project-actions {
  display: flex;
  gap: 10px;
  flex-wrap: wrap;
  margin-top: 6px;
}
.btn-lite {
  display: inline-block;
  padding: 7px 10px;
  border-radius: 10px;
  border: 1px solid rgba(0,0,0,0.18);
  text-decoration: none;
  font-size: 0.92rem;
}
@media (prefers-color-scheme: dark) {
  .btn-lite { border-color: rgba(255,255,255,0.22); }
}

@media (max-width: 860px) {
  .project-card.has-media .project-grid { grid-template-columns: 1fr; } /* stack on small screens */
}
</style>

<div class="projects">

  <!-- 1) No image (single column) -->
  <section class="project-card">
    <h3 class="project-title">Physics-Informed HVAC Controller</h3>
    <div class="project-grid">
      <div class="project-desc">
        <p>Hybrid control approach combining <em>Sparse Identification of Nonlinear Dynamics (SINDy)</em> for system identification with <em>differentiable predictive control (DPC)</em> for offline policy optimization and <em>model-based reinforcement learning (MBRL)</em>. Designed for interpretability and edge-friendly deployment.</p>
      </div>
    </div>
  </section>

  <!-- 2) With image (two columns: text left, image right) -->
  <section class="project-card has-media">
    <h3 class="project-title">Scalable & Secure IoT Data Pipeline for Smart Buildings</h3>
    <div class="project-grid">
      <div class="project-desc">
        <p>End-to-end platform integrating MQTT and Kafka with an ontology-driven Neo4j graph and TimescaleDB for time-series storage. Built preprocessing layers, a data warehouse, REST APIs, and Grafana dashboards. Deployed on Kubernetes (k3s) with a focus on security and observability.</p>
      </div>
      <div class="project-media">
        <img src="/assets/images/data_model.jpg" alt="IoT data model and pipeline overview" loading="lazy" width="960" height="720">
      </div>
    </div>
  </section>

  <!-- 3) No image (single column) -->
  <section class="project-card">
    <h3 class="project-title">LLM-Powered Evidence Extraction & Scoring for Climate Action Plans</h3>
    <div class="project-grid">
      <div class="project-desc">
        <p>Document evaluation pipeline that locates supporting evidence in long PDFs and computes rubric-based scores against predefined indicators. Produces structured JSON with page-level citations for auditability; adaptable to policy, compliance, and technical reports.</p>
      </div>
    </div>
  </section>

  <!-- 4) No image (single column) + multiple code links -->
  <section class="project-card">
    <h3 class="project-title">Sparse Reconstruction of Turbulent Flow from Minimal Sensors</h3>
    <div class="project-grid">
      <div class="project-desc">
        <p>End-to-end framework for reconstructing turbulent flow fields from sparse measurements. Developed a spatiotemporal Transformer (Performer attention) for long-horizon forecasting and a GPU-accelerated tool for sparsity-promoting DMD (sp-DMD). Outputs mapped through complex-valued autoencoders and deep neural networks.</p>
        <div class="project-actions">
          <a class="btn-lite" href="https://github.com/shahin-smv93/ST_Transformer.git" target="_blank" rel="noopener">Code: ST_Transformer</a>
          <a class="btn-lite" href="https://github.com/shahin-smv93/spdmd-tool.git" target="_blank" rel="noopener">Code: spdmd-tool</a>
          <a class="btn-lite" href="https://github.com/shahin-smv93/ComplexAE" target="_blank" rel="noopener">Code: ComplexAE</a>
        </div>
      </div>
    </div>
  </section>

  <!-- 5) With image (two columns: text left, image right) -->
  <section class="project-card has-media">
    <h3 class="project-title">Unified Ontology for Smart Buildings & Cities</h3>
    <div class="project-grid">
      <div class="project-desc">
        <p>Composed and extended standard ontologies to create a unified schema for built-environment data. Built mapping tools to align heterogeneous datasets to the ontology and publish them into Neo4j, enabling consistent metadata, integration, and discovery.</p>
        <div class="project-actions">
          <a class="btn-lite" href="https://github.com/shahin-smv93/ontology-graph-db.git" target="_blank" rel="noopener">Code</a>
        </div>
      </div>
      <div class="project-media">
        <img src="/assets/images/ontology.jpg" alt="Unified ontology and graph mapping" loading="lazy" width="960" height="720">
      </div>
    </div>
  </section>

  <!-- 6) No image (single column) + one code link -->
  <section class="project-card">
    <h3 class="project-title">Map-Matching & City-Scale CO₂ Estimation from Noisy GPS</h3>
    <div class="project-grid">
      <div class="project-desc">
        <p>PostGIS-based map-matching with efficient spatial segmentation and tree-based querying. Developed a segmentation + Fréchet-distance matching approach to compute road-level CO₂. Applied across a large urban road network.</p>
        <div class="project-actions">
          <a class="btn-lite" href="https://github.com/shahin-smv93/transportation_project_map_matching_frechet.git" target="_blank" rel="noopener">Code</a>
        </div>
      </div>
    </div>
  </section>

</div>