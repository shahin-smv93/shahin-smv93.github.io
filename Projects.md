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
.project-grid {
  display: grid;
  grid-template-columns: 0.85fr 1.15fr; /* left media, right text */
  gap: 16px;
  align-items: start;
}
.project-media {
  display: none; /* hidden until you add an image */
}
.project-desc p {
  margin-top: 6px;
  margin-bottom: 10px;
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
  .project-grid { grid-template-columns: 1fr; }
}
</style>

<div class="projects">

  <!-- Project 1 -->
  <section class="project-card">
    <h3 class="project-title">Physics-Informed HVAC Controller</h3>
    <div class="project-grid">
      <div class="project-media">
        <!-- Add an image later:
        <img src="/assets/images/hvac-controller.jpg" alt="HVAC controller visualization" loading="lazy">
        -->
      </div>
      <div class="project-desc">
        <p>Hybrid control approach combining <em>Sparse Identification of Nonlinear Dynamics (SINDy)</em> for system identification with <em>differentiable predictive control (DPC)</em> for offline policy optimization and <em>model-based reinforcement learning (MBRL)</em>. Designed for interpretability and edge-friendly deployment.</p>
        <div class="project-actions">
          <!-- Add links later:
          <a class="btn-lite" href="#" target="_blank" rel="noopener">Paper</a>
          <a class="btn-lite" href="#" target="_blank" rel="noopener">GitHub</a>
          <a class="btn-lite" href="#" target="_blank" rel="noopener">Demo</a>
          -->
        </div>
      </div>
    </div>
  </section>

  <!-- Project 2 -->
  <section class="project-card">
    <h3 class="project-title">Scalable & Secure IoT Data Pipeline for Smart Buildings</h3>
    <div class="project-grid">
      <div class="project-media">
        <!-- <img src="/assets/images/iot-pipeline.jpg" alt="IoT pipeline diagram" loading="lazy"> -->
      </div>
      <div class="project-desc">
        <p>End-to-end platform integrating MQTT and Kafka with an ontology-driven Neo4j graph and TimescaleDB for time-series storage. Built preprocessing layers, a data warehouse, REST APIs, and Grafana dashboards. Deployed on Kubernetes (k3s) with a focus on security and observability.</p>
        <div class="project-actions">
          <!-- <a class="btn-lite" href="#" target="_blank" rel="noopener">GitHub</a> -->
        </div>
      </div>
    </div>
  </section>

  <!-- Project 3 -->
  <section class="project-card">
    <h3 class="project-title">LLM-Powered Evidence Extraction & Scoring for Climate Action Plans</h3>
    <div class="project-grid">
      <div class="project-media">
        <!-- <img src="/assets/images/llm-cap.jpg" alt="LLM pipeline screenshot" loading="lazy"> -->
      </div>
      <div class="project-desc">
        <p>Document evaluation pipeline that locates supporting evidence in long PDFs and computes rubric-based scores against predefined indicators. Produces structured JSON with page-level citations for auditability; adaptable to policy, compliance, and technical reports.</p>
        <div class="project-actions">
          <!-- <a class="btn-lite" href="#" target="_blank" rel="noopener">Paper</a>
          <a class="btn-lite" href="#" target="_blank" rel="noopener">GitHub</a> -->
        </div>
      </div>
    </div>
  </section>

  <!-- Project 4 -->
  <section class="project-card">
    <h3 class="project-title">Sparse Reconstruction of Turbulent Flow from Minimal Sensors</h3>
    <div class="project-grid">
      <div class="project-media">
        <!-- <img src="/assets/images/turbulent-reconstruction.jpg" alt="Flow reconstruction visualization" loading="lazy"> -->
      </div>
      <div class="project-desc">
        <p>End-to-end framework for reconstructing turbulent flow fields from sparse measurements. Developed a spatiotemporal Transformer (Performer attention) for long-horizon forecasting and a GPU-accelerated tool for sparsity-promoting DMD (sp-DMD). Outputs mapped through complex-valued autoencoders and deep neural networks.</p>
        <div class="project-actions">
          <!-- <a class="btn-lite" href="#" target="_blank" rel="noopener">Paper</a>
          <a class="btn-lite" href="#" target="_blank" rel="noopener">GitHub</a> -->
        </div>
      </div>
    </div>
  </section>

  <!-- Project 5 -->
  <section class="project-card">
    <h3 class="project-title">Unified Ontology for Smart Buildings & Cities</h3>
    <div class="project-grid">
      <div class="project-media">
        <!-- <img src="/assets/images/ontology.jpg" alt="Ontology mapping" loading="lazy"> -->
      </div>
      <div class="project-desc">
        <p>Composed and extended standard ontologies to create a unified schema for built-environment data. Built mapping tools to align heterogeneous datasets to the ontology and publish them into Neo4j, enabling consistent metadata, integration, and discovery.</p>
        <div class="project-actions">
          <!-- <a class="btn-lite" href="#" target="_blank" rel="noopener">Docs</a>
          <a class="btn-lite" href="#" target="_blank" rel="noopener">GitHub</a> -->
        </div>
      </div>
    </div>
  </section>

  <!-- Project 6 -->
  <section class="project-card">
    <h3 class="project-title">Map-Matching & City-Scale CO₂ Estimation from Noisy GPS</h3>
    <div class="project-grid">
      <div class="project-media">
        <!-- <img src="/assets/images/map-matching.jpg" alt="Map-matching snapshot" loading="lazy"> -->
      </div>
      <div class="project-desc">
        <p>PostGIS-based map-matching with efficient spatial segmentation and tree-based querying. Developed two approaches to compute road-level CO₂: (1) segmentation + Fréchet-distance matching; (2) enhanced kriging with covariance reduction. Applied across a large urban road network.</p>
        <div class="project-actions">
          <!-- <a class="btn-lite" href="#" target="_blank" rel="noopener">Paper</a>
          <a class="btn-lite" href="#" target="_blank" rel="noopener">GitHub</a> -->
        </div>
      </div>
    </div>
  </section>

</div>