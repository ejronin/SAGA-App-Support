---
layout: page
title: SAGA Documentation
---

<style>
.docs-home-prototype {
  --docs-border: #42474d;
  --docs-panel: #1d2024;
  --docs-panel-hover: #252a30;
  --docs-text: #dfe3e7;
  --docs-muted: #bbc2ca;
  --docs-accent: #7ddfed;
}

.docs-home-prototype .docs-brand-mark {
  margin: 0.25rem 0 0.9rem;
  text-align: center;
}

.docs-home-prototype .docs-brand-mark img {
  display: inline-block;
  width: auto;
  max-width: min(420px, 100%);
  height: auto;
  border: 0;
  box-shadow: none;
}

.docs-home-prototype .docs-home-intro {
  max-width: 70ch;
  margin: 0 auto 1.35rem;
  color: #cfd4da;
  font-size: 1.08rem;
  line-height: 1.55;
  text-align: center;
}

.docs-home-prototype .docs-status {
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

.docs-home-prototype .docs-status strong,
.docs-home-prototype .docs-fact strong {
  color: #f5f7fa;
}

.docs-home-prototype .docs-status span,
.docs-home-prototype .docs-fact span {
  color: #cbd1d7;
}

.docs-home-prototype h2 {
  margin-top: 2.1rem;
  padding-top: 0.25rem;
}

.docs-home-prototype .docs-index-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 0.8rem;
  margin: 1rem 0 2rem;
}

.docs-home-prototype .docs-index-card,
.docs-home-prototype .docs-index-card:visited {
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

.docs-home-prototype .docs-index-card strong {
  display: block;
  margin-bottom: 0.35rem;
  color: #f5f7fa;
  font-size: 1.03rem;
}

.docs-home-prototype .docs-index-card > span:last-child {
  display: block;
  color: var(--docs-muted);
  line-height: 1.45;
}

.docs-home-prototype .docs-index-label {
  display: block;
  margin-bottom: 0.45rem;
  color: var(--docs-accent) !important;
  font-size: 0.73rem;
  font-weight: 700;
  letter-spacing: 0.07em;
  text-transform: uppercase;
}

.docs-home-prototype .docs-index-card:hover,
.docs-home-prototype .docs-index-card:focus-visible {
  color: #f5f7fa;
  background: var(--docs-panel-hover);
  border-color: #5b626a;
  text-decoration: none;
}

.docs-home-prototype .docs-facts {
  margin: 0.8rem 0 2rem;
  border-top: 1px solid var(--docs-border);
}

.docs-home-prototype .docs-fact {
  display: grid;
  grid-template-columns: 150px minmax(0, 1fr);
  gap: 1rem;
  padding: 0.75rem 0;
  border-bottom: 1px solid var(--docs-border);
}

.docs-home-prototype .docs-policy-links {
  margin-bottom: 0;
}

@media screen and (max-width: 780px) {
  .docs-home-prototype .docs-index-grid {
    grid-template-columns: 1fr;
  }
}

@media screen and (max-width: 600px) {
  .docs-home-prototype .docs-status,
  .docs-home-prototype .docs-fact {
    grid-template-columns: 1fr;
    gap: 0.25rem;
  }
}
</style>

<div class="docs-home-prototype">

<p class="docs-brand-mark">
  <img src="assets/saga-for-fusion.png" alt="SAGA for Fusion" width="420">
</p>

<p class="docs-home-intro">Documentation and support for SAGA — Shawn's Assembly Guide Authoring for Autodesk Fusion.</p>

<div class="docs-status" role="status">
  <strong>Release status</strong>
  <span>SAGA 1.0 is in Autodesk Design and Make Marketplace review and release qualification. Public Marketplace availability has not yet been confirmed.</span>
</div>

## Start here

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

## Help and reference

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

## Product information

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

## Policies

<p class="docs-policy-links">[Privacy](privacy.md) · [Licensing](licensing.md) · [Refunds](refunds.md) · [Release and Update Policy](updates.md)</p>

</div>
