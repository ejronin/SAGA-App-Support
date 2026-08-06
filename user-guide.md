---
layout: page
title: User Guide
---

SAGA — Shawn's Assembly Guide Authoring — is an Autodesk Fusion add-in for creating illustrated assembly guides from the model and view already open in Fusion. Projects remain editable and are stored in a normal local folder. When the guide is ready, SAGA creates one complete PDF in that project folder.

For a shorter first-use walkthrough, start with the [Quick Start](quick-start.md).

<div class="page-toc">
<strong>In this guide</strong>
<ul>
  <li><a href="#access-installation-and-startup">Access, installation, and startup</a></li>
  <li><a href="#projects-and-local-storage">Projects and local storage</a></li>
  <li><a href="#project-settings">Project settings</a></li>
  <li><a href="#parts-hardware-tools-and-consumables">Parts, hardware, tools, and consumables</a></li>
  <li><a href="#steps-captures-and-markup">Steps, captures, and markup</a></li>
  <li><a href="#configuration-paths">Configuration paths</a></li>
  <li><a href="#check-project">Check Project</a></li>
  <li><a href="#create-the-pdf">Create the PDF</a></li>
  <li><a href="#marketplace-access">Marketplace access</a></li>
  <li><a href="#logs-help-and-support">Logs, help, and support</a></li>
</ul>
</div>

## Access, installation, and startup

SAGA is distributed through the Autodesk Design and Make Marketplace for 64-bit Windows.

Close Fusion before installing, updating, or removing SAGA. After installation:

1. Open **Utilities > Scripts and Add-Ins**.
2. Select **Add-Ins**.
3. Select **SAGA** and choose **Run**.
4. Use the SAGA toolbar command to reopen the palette during the same Fusion session.

SAGA does not start automatically by default. Fusion may allow you to enable automatic startup later.

<figure class="guide-shot guide-shot--compact">
  <img src="assets/scripts-addins.webp" alt="SAGA selected in Fusion Scripts and Add-Ins">
  <figcaption>SAGA appears as an add-in; automatic startup is intentionally off by default.</figcaption>
</figure>

At launch, SAGA checks the signed-in Fusion account through Autodesk Marketplace. See [Marketplace access](#marketplace-access) for trial, purchase, and offline behavior.

## Projects and local storage

A SAGA project is a folder that keeps the editable project record and its related files together. Depending on the project, the folder may contain:

- Captured Fusion images
- Editable markup records and rendered step images
- Written instructions and notices
- Imported BOM sources
- Project logo and finished-product cover image
- Generated PDF output
- Local diagnostic and recovery information

SAGA does not upload the Fusion model or project content to a SAGA-operated server. Keep the complete project folder together when moving, backing up, or archiving a guide.

### Create a project

On **Project**:

1. Enter the product name.
2. Enter the product and manual revisions.
3. Enter the manual title and author.
4. Choose the parent folder for new projects.
5. Select **New Project**.

The product revision identifies the physical design. The manual revision identifies the instruction document. They may change independently.

<figure class="guide-shot guide-shot--compact">
  <img src="assets/project-setup.webp" alt="Project identity, revisions, author, and local project location in SAGA">
  <figcaption>Project identity and local storage settings.</figcaption>
</figure>

### Open and save

Use **Open** to select an existing SAGA project folder. Use **Save** after meaningful work and before closing Fusion.

Generating a PDF does not lock the project. A later successful publication replaces the prior PDF with the current version.

## Project settings

### Cover assets

A project may include one logo and one finished-product image. SAGA copies selected images into the project's `assets` folder so the project does not depend on the original file locations.

### Capture settings

Capture settings apply to new Fusion viewport captures:

- Width and height
- Delay before capture
- Anti-aliasing
- Transparent background

The default 2560 × 1440 capture is suitable for most manuals. Higher resolutions increase project size and PDF-generation time.

When **Transparent background** is enabled, SAGA asks Fusion for an alpha-capable PNG and verifies that the result supports transparency. The setting is saved with the project and can be changed later. Existing captures do not change automatically; recapture a step when a different background treatment is required.

## Parts, hardware, tools, and consumables

The **Parts** tab is both an item catalog and a practical bill of materials. Use it for:

- Printed or fabricated parts
- Purchased hardware
- Tools
- Adhesives, lubricant, and other consumables

A clear item name is the only essential identifier. Part number, supplier, description, notes, marker type, and fixed project quantity are optional.

### Add an item manually

1. Open **Parts**.
2. Select **Add Item**.
3. Choose the category.
4. Enter the name and unit.
5. Add a part number or fixed total quantity when needed.
6. Choose a default visual marker when useful.
7. Save the item.

### Import a BOM

SAGA imports CSV and XLSX sources and copies the imported file into the project. The source must contain a recognized name column such as `Name`, `Item Name`, or `Part Name`.

The import may also use columns for category, quantity, unit, item number, description, supplier, notes, and visual marker.

[Download the SAGA BOM import template](assets/SAGA-BOM-Import-Template.csv).

### Quantity behavior

A fixed project quantity enables allocation checks. Step assignments and BOM-linked callouts may either:

- **Install or use quantity** — counts against the planned total
- **Reference only** — identifies an item without consuming another unit

Use reference-only callouts when the same installed item must be identified again later or along an alternate configuration path.

## Steps, captures, and markup

Open **Steps** and select **New Step**. Each step has three work areas: **Details**, **Image**, and **Markup**.

### Step details

Give each step a short operation title, such as “Install the hinge rod,” and write the instruction in direct, actionable language.

A step can also contain:

- Parts, hardware, tools, and consumables used at that step
- Information, caution, warning, do-not, inspect, and check notices
- An optional printed step number for linear projects
- A configuration split point

### Capture the Fusion view

Before selecting **Capture View**:

1. Set the model position and camera in Fusion.
2. Show or hide components as needed.
3. Choose the visual style and background treatment.
4. Confirm the active step.
5. Capture the view.

Replacing a capture moves the previous source image to the project's trash folder and clears markup tied to the old image.

### Markup tools

SAGA markup remains editable after the project is saved. Available tools include:

- Arrow
- Leader or alignment line
- Text label
- BOM-linked part callout
- Visual marker

Use markup only where it improves understanding. The Fusion capture should remain the main source of visual information.

### BOM-linked part callouts

A part callout can pull its label and marker from the project catalog. Set the quantity shown and choose whether the callout installs or uses that quantity, or is reference-only.

Select **Apply Markup to Step** after changing image markup. SAGA retains both the editable markup records and the rendered image used in the PDF. Save the project before closing Fusion.

When leaving Markup with unapplied changes, SAGA offers:

- **Apply and Continue**
- **Discard Changes**
- **Cancel**

Discard returns to the last applied markup; it does not delete the original Fusion capture.

## Configuration paths

Configurations are optional. Use them when the guide has a shared opening sequence followed by alternate assembly choices and, optionally, a shared finish.

SAGA 1.0 supports one split and up to five paths. Nested splits are not supported.

To create a split:

1. Select the last shared step before the alternatives begin.
2. Choose **Create Split Here**.
3. Name the first two paths.
4. Add more paths when needed.
5. Select a path while creating its branch steps.

SAGA calculates path-specific printed step numbers and adds PDF links so readers can move from the shared sequence to the correct branch.

## Check Project

Open **Check Project** before publication.

- **Errors** must be corrected before PDF generation.
- **Warnings** should be reviewed but do not block publication.

Checks cover required project information, step images and instructions, configuration consistency, BOM allocation, assets, and publication readiness. A step-related result opens the affected step.

## Create the PDF

On **PDF**:

1. Choose the page size and orientation.
2. Choose whether to include the cover page.
3. Choose whether to include contents and links.
4. Choose whether to include the bill of materials.
5. Select **Generate PDF**.

SAGA creates one complete PDF directly in the project folder. The PDF may contain the cover, linked contents, bookmarks, configuration links, step notices, marked-up images, step-specific item lists, and total BOM.

Large, high-resolution guides may take about a minute to compile. If Windows reports that the output is in use, close the PDF in its viewer and generate it again.

<figure class="guide-shot guide-shot--pdf">
  <img src="assets/sample-output.jpg" alt="Example SAGA assembly guide output">
  <figcaption>Example SAGA output. The full demonstration guide is included with the Autodesk Marketplace listing.</figcaption>
</figure>

## Marketplace access

SAGA is a paid, one-time-purchase Marketplace application. The Autodesk listing offers Autodesk's optional 30-day trial.

- Autodesk controls both trial and purchased access.
- SAGA does not run a separate local trial clock.
- Trial output is not watermarked, and customer branding remains enabled.
- The palette reports only whether Marketplace access is active; Autodesk does not provide SAGA with the entitlement type or remaining trial time.

SAGA checks the signed-in Fusion account through Autodesk's Entitlement API. A successful result may be used for up to 24 hours if Autodesk's service is temporarily unavailable. A completed negative Autodesk result takes effect immediately.

When access ends, authoring and PDF publication are disabled until Autodesk reports valid access again. Existing projects and previously generated PDFs are not deleted or altered.

When the palette shows **Access required**:

1. Confirm that Fusion is signed in with the Autodesk account used for the trial or purchase.
2. Complete the Marketplace trial or purchase using that account.
3. Return to SAGA and select **Check again**.

## Logs, help, and support

Select **Help** in the palette or press **F1 while the SAGA palette has keyboard focus**. Fusion routes F1 to the active pane, so SAGA help does not open while the Fusion canvas has focus.

SAGA writes local diagnostic logs under:

```text
%LOCALAPPDATA%\SAGA\logs
```

When requesting support, include:

- SAGA version
- Fusion version
- Windows version
- The exact error message
- Steps that reproduce the issue
- A screenshot or local SAGA log when useful

Remove confidential project information before sending logs or screenshots unless it is necessary to diagnose the issue.

Support: **sagaappsupport@gmail.com**

See the [Support Policy](support.md), [Privacy Policy](privacy.md), and [Troubleshooting](troubleshooting.md) pages for more information.
