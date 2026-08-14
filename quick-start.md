---
layout: page
title: Quick Start
---

This walkthrough takes you from first launch to a finished PDF. For expanded control-by-control workflow detail, continue with the [User Guide](user-guide.md).

<div class="notice-box">
<strong>Release status:</strong> SAGA 1.0 is currently in Autodesk Design and Make Marketplace review and release qualification. These steps describe the intended Marketplace release workflow; public Marketplace availability has not yet been confirmed.
</div>

<div class="notice-box">
<strong>Before you begin:</strong> open the Fusion design you want to document and sign in to Fusion with the same Autodesk account used for the SAGA trial or purchase.
</div>

## 1. Install and start SAGA

Install SAGA through the Autodesk Design and Make Marketplace. Close Fusion before installing, updating, or removing the add-in.

SAGA does not start automatically by default. In Fusion:

1. Open **Utilities > Scripts and Add-Ins**.
2. Select **Add-Ins**.
3. Select **SAGA** and choose **Run**.
4. Use the SAGA command in the Fusion toolbar to reopen the palette during the same session.

<figure class="guide-shot guide-shot--compact">
  <img src="assets/scripts-addins.webp" alt="SAGA selected in Fusion Scripts and Add-Ins">
  <figcaption>SAGA listed in Fusion with automatic startup left off.</figcaption>
</figure>

## 2. Confirm Marketplace access

SAGA uses Autodesk Marketplace entitlement verification for both the Free 30-Day Trial and purchased access.

- **Access active** means the signed-in Autodesk account can use SAGA.
- **Access required** means the account does not currently have an active trial or purchase entitlement.

When access is required, start the Marketplace trial or purchase SAGA using the same Autodesk account, return to Fusion, and select **Check again**. SAGA does not run a separate local trial clock.

## 3. Create or open a project

On **Project**:

1. Enter the product name, product revision, manual revision, title, and author.
2. Choose the parent folder for new projects.
3. Select **New Project**.
4. Add a logo and finished-product image when useful.
5. Review the capture settings, including transparent background.

Use **Open** to continue an existing SAGA project folder.

SAGA keeps the editable project, captures, imported BOM files, cover assets, and generated PDF together in the local project folder.

## 4. Add parts, hardware, tools, and consumables

Open **Parts** to add items manually or import a CSV/XLSX bill of materials. A part number is optional unless the assembly depends on an exact component.

The import source needs a recognized name column such as `Name`, `Item Name`, or `Part Name`.

[Download the SAGA BOM import template](assets/SAGA-BOM-Import-Template.csv).

## 5. Create the first step and capture the view

1. Open **Steps** and select **New Step**.
2. Enter a short operation title and direct instruction.
3. Assign any parts or tools used in that step.
4. Position the model and camera in Fusion.
5. Show or hide components as needed.
6. Open the step's **Image** area and select **Capture View**.

## 6. Add markup

Open **Markup** and add only the visual guidance the reader needs. SAGA provides arrows, leaders, alignment lines, labels, visual markers, and BOM-linked part callouts.

Select **Apply Markup to Step** after changing the image, then save the project.

<div class="notice-box">
<strong>Before leaving Markup:</strong> if SAGA asks what to do with unapplied changes, choose <strong>Apply and Continue</strong> when you want to keep the current image and markup. <strong>Discard Changes</strong> can move the active step image to the project's trash, which means you may need to recapture the step before markup can continue. See <a href="{{ '/user-guide.html#leaving-markup-with-unapplied-changes' | relative_url }}">Leaving Markup with unapplied changes</a> for the exact behavior and recovery steps.
</div>

## 7. Check the project

Open **Check Project** and run the check.

- Correct every error before publication.
- Review warnings and leave them only when intentional.

## 8. Generate the PDF

1. Open **PDF**.
2. Choose page size and orientation.
3. Choose the optional cover, contents, links, and total BOM.
4. Select **Generate PDF**.

The complete PDF is written directly into the project folder. The demonstration guide and listing screenshots are part of the Marketplace submission materials. Public downloads will be added after Marketplace review is complete.

## Help while you work

Select **Help** in the SAGA palette or press **F1 while the palette has keyboard focus**. F1 is handled by the active Fusion pane, so it will not open SAGA help while the Fusion canvas has focus.

Continue with the [User Guide](user-guide.md) for additional detail on capture settings, BOM allocation, notices, configuration paths, validation rules, entitlement behavior, logs, and support.
