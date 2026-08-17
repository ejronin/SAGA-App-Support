---
layout: page
title: SAGA
---

<style>
.saga-platform-home {
  --docs-border: #42474d;
  --docs-panel: #1d2024;
  --docs-panel-hover: #252a30;
  --docs-text: #dfe3e7;
  --docs-muted: #bbc2ca;
  --docs-accent: #7ddfed;
}

.saga-platform-home .saga-master {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 1.2rem;
  margin: 0.4rem auto 1.4rem;
}

.saga-platform-home .saga-master img {
  width: min(170px, 28vw);
  height: auto;
  border: 0;
  box-shadow: none;
}

.saga-platform-home .saga-master-name {
  color: #f5f7fa;
  font-family: Montserrat, "Arial Black", "Helvetica Neue", sans-serif;
  font-size: clamp(3rem, 8vw, 6.2rem);
  font-weight: 800;
  letter-spacing: 0.015em;
  line-height: 0.95;
}

.saga-platform-home .platform-intro {
  max-width: 66ch;
  margin: 0 auto 2rem;
  color: #cfd4da;
  font-size: 1.08rem;
  line-height: 1.6;
  text-align: center;
}

.saga-platform-home .platform-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 1rem;
  margin: 1rem 0 2.25rem;
}

.saga-platform-home .platform-card,
.saga-platform-home .platform-card:visited {
  display: flex;
  min-width: 0;
  min-height: 100%;
  flex-direction: column;
  box-sizing: border-box;
  padding: 1rem;
  color: var(--docs-text);
  background: var(--docs-panel);
  border: 1px solid var(--docs-border);
  border-radius: 7px;
  text-decoration: none;
  transition: border-color 120ms ease, background 120ms ease, transform 120ms ease;
}

.saga-platform-home .platform-card:hover,
.saga-platform-home .platform-card:focus-visible {
  color: #f5f7fa;
  background: var(--docs-panel-hover);
  border-color: #626a73;
  text-decoration: none;
  transform: translateY(-2px);
}

.saga-platform-home .platform-card img {
  display: block;
  width: 100%;
  height: auto;
  margin: 0 auto 0.9rem;
  border: 0;
  box-shadow: none;
}

.saga-platform-home .platform-status {
  display: inline-block;
  align-self: flex-start;
  margin-bottom: 0.65rem;
  padding: 0.27rem 0.55rem;
  color: #dff8fb;
  background: #17353a;
  border: 1px solid #2c6972;
  border-radius: 999px;
  font-size: 0.7rem;
  font-weight: 800;
  letter-spacing: 0.06em;
  text-transform: uppercase;
}

.saga-platform-home .platform-status.coming-soon {
  color: #fff0df;
  background: #4a2c12;
  border-color: #8c5320;
}

.saga-platform-home .platform-card strong {
  margin-bottom: 0.45rem;
  color: #f5f7fa;
  font-size: 1.05rem;
}

.saga-platform-home .platform-card > span:last-child {
  color: var(--docs-muted);
  line-height: 1.5;
}

.saga-platform-home .platform-card .platform-action {
  margin-top: auto;
  padding-top: 1rem;
  color: var(--docs-accent);
  font-weight: 700;
}

.saga-platform-home .platform-card.blender .platform-action {
  color: #f3a14c;
}

.saga-platform-home h2 {
  margin-top: 2rem;
}

.saga-platform-home .difference-table {
  margin: 1rem 0 2rem;
  border-top: 1px solid var(--docs-border);
}

.saga-platform-home .difference-row {
  display: grid;
  grid-template-columns: 170px repeat(2, minmax(0, 1fr));
  gap: 1rem;
  padding: 0.85rem 0;
  border-bottom: 1px solid var(--docs-border);
}

.saga-platform-home .difference-row strong {
  color: #f5f7fa;
}

.saga-platform-home .difference-row span {
  color: #cbd1d7;
  line-height: 1.5;
}

.saga-platform-home .home-note {
  margin-top: 2rem;
  color: #aeb5bd;
  font-size: 0.9rem;
  line-height: 1.5;
}

@media screen and (max-width: 760px) {
  .saga-platform-home .platform-grid {
    grid-template-columns: 1fr;
  }

  .saga-platform-home .difference-row {
    grid-template-columns: 1fr;
    gap: 0.35rem;
  }
}

@media screen and (max-width: 520px) {
  .saga-platform-home .saga-master {
    gap: 0.7rem;
  }

  .saga-platform-home .saga-master img {
    width: 105px;
  }
}
</style>

<div class="saga-platform-home">

<div class="saga-master" aria-label="SAGA">
  <img src="{{ '/assets/SAGA_BookOnly_Transparent_512x512.png' | relative_url }}" alt="">
  <span class="saga-master-name">SAGA</span>
</div>

<p class="platform-intro">SAGA turns 3D maker projects into clear, structured assembly guides. Choose the host application that matches the project you're documenting.</p>

<div class="platform-grid">
  <a class="platform-card fusion" href="{{ '/fusion/' | relative_url }}">
    <img src="{{ '/assets/SAGA for Fusion.png' | relative_url }}" alt="SAGA for Fusion">
    <span class="platform-status">Documentation live</span>
    <strong>For Autodesk Fusion workflows</strong>
    <span>Build illustrated guides around Fusion projects with SAGA projects, parts and BOMs, captured Steps, markup, configuration paths, validation, and PDF publication.</span>
    <span class="platform-action">Open Fusion documentation →</span>
  </a>

  <a class="platform-card blender" href="{{ '/blender/' | relative_url }}">
    <img src="{{ '/assets/SAGA for Blender.png' | relative_url }}" alt="SAGA for Blender">
    <span class="platform-status coming-soon">Coming Soon</span>
    <strong>For Blender-based maker projects</strong>
    <span>Bring SAGA's guide-authoring discipline to model kits, props, figures, articulated projects and other physical builds using Blender-native arrangements, visualization, capture, annotations and publication.</span>
    <span class="platform-action">Preview SAGA for Blender →</span>
  </a>
</div>

<h2>Same SAGA core, tuned to the host</h2>

<div class="difference-table">
  <div class="difference-row">
    <strong>Authoring environment</strong>
    <span><b>Fusion:</b> SAGA works around the Fusion project and its captured assembly views.</span>
    <span><b>Blender:</b> SAGA adds a Blender-native workspace around the scene and saved Step arrangements.</span>
  </div>
  <div class="difference-row">
    <strong>Instructional visuals</strong>
    <span><b>Fusion:</b> capture the prepared Fusion view, then add SAGA markup and callouts.</span>
    <span><b>Blender:</b> save the Step arrangement, choose Normal, Isolate, Ghost, Highlight New or Show All, then capture and optionally annotate.</span>
  </div>
  <div class="difference-row">
    <strong>Alternatives</strong>
    <span><b>Fusion:</b> one configuration split can create alternate guide paths when needed.</span>
    <span><b>Blender:</b> optional option groups and branch paths support alternate configurations, including nested branches and rejoining common Steps.</span>
  </div>
  <div class="difference-row">
    <strong>Output goal</strong>
    <span><b>Fusion:</b> a polished assembly-guide PDF with optional BOM content.</span>
    <span><b>Blender:</b> a publication package built around the assembly manual, BOM outputs, publication data and an optional shareable ZIP.</span>
  </div>
</div>

<p class="home-note">Fusion and Blender product names and marks are shown only to identify the host applications supported by the respective SAGA versions.</p>

</div>
