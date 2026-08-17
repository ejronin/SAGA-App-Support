---
layout: page
title: SAGA for Blender
permalink: /blender/
---

<style>
.blender-coming-soon {
  --docs-border: #42474d;
  --docs-panel: #1d2024;
  --docs-panel-strong: #23272c;
  --docs-text: #dfe3e7;
  --docs-muted: #bbc2ca;
  --docs-accent: #7ddfed;
  --blender-accent: #f28c28;
}

.blender-coming-soon .platform-brand {
  margin: 0.25rem 0 1rem;
  text-align: center;
}

.blender-coming-soon .platform-brand img {
  display: inline-block;
  width: auto;
  max-width: min(720px, 100%);
  height: auto;
  border: 0;
  box-shadow: none;
}

.blender-coming-soon .coming-soon-badge {
  display: table;
  margin: 0 auto 1.15rem;
  padding: 0.34rem 0.72rem;
  color: #fff3e6;
  background: #4a2c12;
  border: 1px solid #8c5320;
  border-radius: 999px;
  font-size: 0.78rem;
  font-weight: 800;
  letter-spacing: 0.07em;
  text-transform: uppercase;
}

.blender-coming-soon .platform-intro {
  max-width: 74ch;
  margin: 0 auto 1.5rem;
  color: #d6dbe0;
  font-size: 1.09rem;
  line-height: 1.6;
  text-align: center;
}

.blender-coming-soon .overview-panel {
  margin: 1.25rem 0 2rem;
  padding: 1.1rem 1.2rem;
  background: var(--docs-panel);
  border: 1px solid var(--docs-border);
  border-left: 3px solid var(--blender-accent);
  border-radius: 6px;
}

.blender-coming-soon .overview-panel strong {
  color: #f5f7fa;
}

.blender-coming-soon h2 {
  margin-top: 2.2rem;
}

.blender-coming-soon .difference-grid,
.blender-coming-soon .docs-roadmap {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 0.85rem;
  margin: 1rem 0 2rem;
}

.blender-coming-soon .difference-card,
.blender-coming-soon .roadmap-card {
  box-sizing: border-box;
  padding: 1rem 1.05rem;
  background: var(--docs-panel);
  border: 1px solid var(--docs-border);
  border-radius: 6px;
}

.blender-coming-soon .difference-card strong,
.blender-coming-soon .roadmap-card strong {
  display: block;
  margin-bottom: 0.38rem;
  color: #f5f7fa;
}

.blender-coming-soon .difference-card span,
.blender-coming-soon .roadmap-card span {
  color: var(--docs-muted);
  line-height: 1.5;
}

.blender-coming-soon .roadmap-card {
  position: relative;
  padding-top: 2.05rem;
}

.blender-coming-soon .roadmap-card::before {
  content: "Coming soon";
  position: absolute;
  top: 0.72rem;
  left: 1.05rem;
  color: #f5a24d;
  font-size: 0.69rem;
  font-weight: 800;
  letter-spacing: 0.07em;
  text-transform: uppercase;
}

.blender-coming-soon .workflow-line {
  margin: 1rem 0 2rem;
  padding: 1rem 1.1rem;
  color: #d4dae0;
  background: var(--docs-panel-strong);
  border: 1px solid var(--docs-border);
  border-radius: 6px;
  line-height: 1.65;
}

.blender-coming-soon .workflow-line strong {
  color: #f5f7fa;
}

.blender-coming-soon .platform-back {
  margin-top: 2rem;
  color: #aeb5bd;
  font-size: 0.94rem;
}

@media screen and (max-width: 720px) {
  .blender-coming-soon .difference-grid,
  .blender-coming-soon .docs-roadmap {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="blender-coming-soon">

<p class="platform-brand">
  <img src="{{ '/assets/SAGA for Blender.png' | relative_url }}" alt="SAGA for Blender">
</p>

<span class="coming-soon-badge">Coming Soon</span>

<p class="platform-intro">SAGA for Blender brings structured assembly-guide authoring into Blender while leaving Blender's normal modeling and editing environment intact. It is being built for makers who need to turn complex 3D projects into clear, repeatable, publication-ready instructions.</p>

<div class="overview-panel">
  <strong>The same SAGA goal, adapted to Blender.</strong> Fusion and Blender solve different kinds of 3D work, so SAGA does not force them into the same interface. Both versions focus on clear parts, ordered Steps, useful visuals, validation, and professional guide output; each version uses the workflow that fits its host application.
</div>

<h2>How the Blender version differs</h2>

<div class="difference-grid">
  <div class="difference-card">
    <strong>Built around Blender scenes</strong>
    <span>SAGA adds a Blender-native authoring workspace around the scene instead of replacing the modeling environment. Arrange the project in 3D, save the intended Step state, choose the instructional visualization, and capture it.</span>
  </div>

  <div class="difference-card">
    <strong>Made for a broader maker mix</strong>
    <span>Project profiles give useful starting context for terrain and model kits, cosplay and props, figures and statues, articulated or kinetic work, and general projects without splitting SAGA into separate products.</span>
  </div>

  <div class="difference-card">
    <strong>Arrangement-aware Steps</strong>
    <span>Each Step can track the parts being used, its saved arrangement, the current visualization, capture state, and optional annotations. If the arrangement changes after capture, SAGA can flag the Step for recapture.</span>
  </div>

  <div class="difference-card">
    <strong>Options when a build really needs them</strong>
    <span>Options and branches are available for alternate configurations, including nested paths and rejoining common Steps, but they stay out of the way for straightforward guides.</span>
  </div>
</div>

<h2>What the workflow looks like</h2>

<div class="workflow-line"><strong>Project → Parts &amp; Materials → Starting Arrangement → Steps → Parts Used → Arrangement → Visualization → Capture → optional Annotations → Review / Validate → Publication</strong></div>

<p>Publication is designed to produce the assembly manual together with BOM and publication-package outputs, with an optional shareable ZIP after a successful build.</p>

<h2>Documentation being prepared</h2>

<div class="docs-roadmap">
  <div class="roadmap-card">
    <strong>Quick Start</strong>
    <span>A direct first-project path from opening the SAGA workspace through a built publication.</span>
  </div>
  <div class="roadmap-card">
    <strong>User Guide</strong>
    <span>The complete guided workflow, including project profiles, parts, arrangements, visualization, capture, annotations, options and publication.</span>
  </div>
  <div class="roadmap-card">
    <strong>Troubleshooting</strong>
    <span>Recovery guidance for incomplete Steps, Needs Recapture, project linking, publication validation and other actionable states.</span>
  </div>
  <div class="roadmap-card">
    <strong>FAQ</strong>
    <span>Platform, workflow, release and common-use questions once the public release details are locked.</span>
  </div>
</div>

<p>The documentation structure is already reserved here. As the Blender release is finalized, the completed pages will be connected to this overview without changing the platform path.</p>

<p class="platform-back"><a href="{{ '/' | relative_url }}">← Back to SAGA platforms</a> · <a href="{{ '/fusion/' | relative_url }}">Open SAGA for Fusion documentation</a></p>

</div>
