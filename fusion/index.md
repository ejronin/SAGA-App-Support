---
layout: page
title: SAGA for Fusion
permalink: /fusion/
---

<style>
.platform-doc-home {
  --docs-border: #42474d;
  --docs-panel: #1d2024;
  --docs-panel-hover: #252a30;
  --docs-text: #dfe3e7;
  --docs-muted: #bbc2ca;
  --docs-accent: #7ddfed;
}

.platform-doc-home .platform-brand {
  margin: 0.25rem 0 1rem;
  text-align: center;
}

.platform-doc-home .platform-brand img {
  display: inline-block;
  width: auto;
  max-width: min(640px, 100%);
  height: auto;
  border: 0;
  box-shadow: none;
}

.platform-doc-home .platform-intro {
  max-width: 70ch;
  margin: 0 auto 1.35rem;
  color: #cfd4da;
  font-size: 1.08rem;
  line-height: 1.55;
  text-align: center;
}

.platform-doc-home .docs-status {
  display: grid;
  grid-template-columns: 125px minmax(0, 1fr);
  gap: 1rem;
  margin: 1rem 0 2rem;
  padding: 0.85rem 1rem;
  background: var(--docs-panel);
  border: 1px solid var(--docs-border);
  border-left: 3px solid #0ea5b7;
  border-radius: 5px;
}

.platform-doc-home .docs-status strong,
.platform-doc-home .docs-fact strong {
  color: #f5f7fa;
}

.platform-doc-home .docs-status span,
.platform-doc-home .docs-fact span {
  color: #cbd1d7;
}

.platform-doc-home h2 {
  margin-top: 2.1rem;
  padding-top: 0.25rem;
}

.platform-doc-home .docs-index-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 0.8rem;
  margin: 1rem 0 2rem;
}

.platform-doc-home .docs-index-card,
.platform-doc-home .docs-index-card:visited {
  display: block;
  min-height: 100%;
  box-sizing: border-box;
  padding: 1rem 1.05rem;
  color: var(--docs-text);
  background: var(--docs-panel);
  border: 1px solid var(--docs-border);
  border-radius: 6px;
  text-decoration: none;
}

.platform-doc-home .docs-index-card strong {
  display: block;
  margin-bottom: 0.35rem;
  color: #f5f7fa;
  font-size: 1.03rem;
}

.platform-doc-home .docs-index-card > span:last-child {
  display: block;
  color: var(--docs-muted);
  line-height: 1.45;
}

.platform-doc-home .docs-index-label {
  display: block;
  margin-bottom: 0.45rem;
  color: var(--docs-accent) !important;
  font-size: 0.73rem;
  font-weight: 700;
  letter-spacing: 0.07em;
  text-transform: uppercase;
}

.platform-doc-home .docs-index-card:hover,
.platform-doc-home .docs-index-card:focus-visible {
  color: #f5f7fa;
  background: var(--docs-panel-hover);
  border-color: #5b626a;
  text-decoration: none;
}

.platform-doc-home .docs-facts {
  margin: 0.8rem 0 2rem;
  border-top: 1px solid var(--docs-border);
}

.platform-doc-home .docs-fact {
  display: grid;
  grid-template-columns: 150px minmax(0, 1fr);
  gap: 1rem;
  padding: 0.75rem 0;
  border-bottom: 1px solid var(--docs-border);
}

.platform-doc-home .docs-policy-links {
  margin-bottom: 0;
}

.platform-doc-home .platform-back {
  margin-top: 2rem;
  color: #aeb5bd;
  font-size: 0.94rem;
}

@media screen and (max-width: 780px) {
  .platform-doc-home .docs-index-grid {
    grid-template-columns: 1fr;
  }
}

@media screen and (max-width: 600px) {
  .platform-doc-home .docs-status,
  .platform-doc-home .docs-fact {
    grid-template-columns: 1fr;
    gap: 0.25rem;
  }
}
</style>

<div class="platform-doc-home">

<p class="platform-brand">
  <img src="{{ '/assets/SAGA for Fusion.png' | relative_url }}" alt="SAGA for Fusion">
</p>

<p class="platform-intro">Create clear, illustrated assembly guides directly from Autodesk Fusion with SAGA's project, parts, step, markup, configuration, and PDF-authoring workflow.</p>

<div class="docs-status" role="status">
  <strong>Release status</strong>
  <span>SAGA 1.0 is in Autodesk Design and Make Marketplace review and release qualification. Public Marketplace availability has not yet been confirmed.</span>
</div>

<h2>Start here</h2>

<div class="docs-index-grid">
  <a class="docs-index-card" href="{{ '/quick-start.html' | relative_url }}">
    <span class="docs-index-label">Getting started</span>
    <strong>Quick Start</strong>
    <span>Go from first launch to a finished SAGA PDF.</span>
  </a>

  <a class="docs-index-card" href="{{ '/user-guide.html' | relative_url }}">
    <span class="docs-index-label">Full reference</span>
    <strong>User Guide</strong>
    <span>Projects, captures, BOMs, steps, markup, configuration paths, publication, and access.</span>
  </a>

  <a class="docs-index-card" href="{{ '/troubleshooting.html' | relative_url }}">
    <span class="docs-index-label">Recovery</span>
    <strong>Troubleshooting</strong>
    <span>Work through common startup, project, capture, publication, and Marketplace-access problems.</span>
  </a>
</div>

<h2>Help and reference</h2>

<div class="docs-index-grid">
  <a class="docs-index-card" href="{{ '/faq.html' | relative_url }}">
    <strong>FAQ</strong>
    <span>Common product, platform, trial, licensing, and workflow questions.</span>
  </a>

  <a class="docs-index-card" href="{{ '/support.html' | relative_url }}">
    <strong>Support</strong>
    <span>Support hours, coverage, and what to include when reporting a problem.</span>
  </a>

  <a class="docs-index-card" href="{{ '/release-notes.html' | relative_url }}">
    <strong>Release Notes</strong>
    <span>Current release information and documented changes.</span>
  </a>
</div>

<h2>Product information</h2>

<div class="docs-facts" role="list">
  <div class="docs-fact" role="listitem">
    <strong>Platform</strong>
    <span>Windows with Autodesk Fusion.</span>
  </div>
  <div class="docs-fact" role="listitem">
    <strong>Project storage</strong>
    <span>SAGA projects, captures, guide content, and generated PDFs stay in the local folders you choose.</span>
  </div>
  <div class="docs-fact" role="listitem">
    <strong>Marketplace access</strong>
    <span>One-time purchase with Autodesk's Free 30-Day Trial option enabled for the submitted release.</span>
  </div>
  <div class="docs-fact" role="listitem">
    <strong>Support</strong>
    <span>Email <a href="mailto:sagaappsupport@gmail.com">sagaappsupport@gmail.com</a>.</span>
  </div>
</div>

<h2>Policies</h2>

<p class="docs-policy-links"><a href="{{ '/privacy.html' | relative_url }}">Privacy</a> · <a href="{{ '/licensing.html' | relative_url }}">Licensing</a> · <a href="{{ '/refunds.html' | relative_url }}">Refunds</a> · <a href="{{ '/updates.html' | relative_url }}">Release and Update Policy</a></p>

<p class="platform-back"><a href="{{ '/' | relative_url }}">← Choose another SAGA platform</a></p>

</div>
