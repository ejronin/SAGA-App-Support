---
layout: page
title: Quick Start
---

# SAGA Quick Start

This walkthrough creates a basic assembly guide from an open Fusion design. The [User Guide](user-guide.md) covers the complete workflow.

## 1. Install and start SAGA

Install SAGA through the Autodesk Design and Make Marketplace. Close Fusion before installing, updating, or removing the add-in.

SAGA does not start automatically by default. In Fusion:

1. Open **Utilities > Scripts and Add-Ins**.
2. Select **Add-Ins**.
3. Select **SAGA** and run it.
4. Use the SAGA command in the toolbar to open the palette.

![SAGA selected in Scripts and Add-Ins](assets/scripts-addins.webp)

## 2. Create a project

On **Project**:

1. Enter the product name, product revision, manual revision, title, and author.
2. Choose the parent folder for new projects.
3. Select **New Project**.
4. Add a logo and finished-product image when wanted.
5. Review the capture settings.

SAGA creates a local project folder and keeps the editable project, captures, assets, imported BOM files, and PDF together.

![Project setup](assets/project-setup.webp)

## 3. Add parts when useful

Open **Parts** to add printed parts, hardware, tools, and consumables. A part number is optional unless the assembly depends on an exact component.

Use **Import CSV/XLSX** to import an existing BOM, or [download the SAGA BOM template](assets/SAGA-BOM-Import-Template.csv).

![Parts and BOM catalog](assets/parts-bom.webp)

## 4. Add the first step

1. Open **Steps**.
2. Select **New Step**.
3. Enter a short operation title and the instruction.
4. Assign any parts used at the step.
5. In Fusion, position the model exactly as the reader should see it.
6. Open the step's **Image** area and select **Capture View**.

## 5. Add markup

Open **Markup** and add only the visual guidance the reader needs. SAGA provides arrows, leaders, alignment lines, labels, visual markers, and BOM-linked part callouts.

Select **Apply Markup to Step** after making image changes. Then save the project so the markup remains editable after Fusion closes.

![BOM-linked part callout](assets/bom-callout.webp)

## 6. Check the project

Open **Check Project** and select **Check Project**.

- Fix every error.
- Review warnings and leave them only when intentional.

## 7. Generate the PDF

1. Open **PDF**.
2. Choose page size and orientation.
3. Choose the optional cover, contents, links, and BOM sections.
4. Select **Generate PDF**.

The complete PDF is written directly into the project folder.

![PDF publication settings](assets/pdf-generation.webp)

[Download the SAGA demonstration assembly guide](assets/SAGA-Demo-Assembly-Guide.pdf)

## Next steps

Continue with the [User Guide](user-guide.md) for transparent captures, BOM allocation, notices, configuration paths, validation rules, licensing, logs, and support.
