# User Guide production replacement notes

This file is a controlled writing draft for the next GitHub pass. It does not replace the repository file by itself.

## Project settings — Capture settings

Capture settings apply to new or replacement viewport captures.

- The default capture size shown in the owner workflow is **2560 × 1440**.
- **Anti-alias** is enabled in the demonstrated default setup.
- **Transparent background is off on the first run.** Enable it before the first transparent capture you want to make.
- After you select Transparent background, SAGA remembers that setting for later runs. You may still toggle it for an individual capture.
- Changing a setting does not change an existing captured step image. Recapture that step when it needs the new setting.
- **Capture diagnostics** is a troubleshooting tool, not part of the normal authoring sequence. Use it only when capture behavior appears incorrect.

## Parts, hardware, tools, and consumables

The catalog category choices demonstrated in SAGA are **Part, Hardware, Tool, and Consumable**.

A catalog item may include:
- item or part number;
- category;
- name;
- size/specification;
- optional fixed total quantity;
- unit;
- description;
- supplier;
- default visual marker;
- notes.

A fixed total quantity enables allocation checking. Assignments and BOM-aware callouts can consume that quantity when they represent an installed/used item. A reference-only visual identification does not consume another unit.

## Steps, captures, instructions, and markup

A standard step is completed in this order:

1. Create the step.
2. On **Details**, give the step a useful title and assign the parts, hardware, tools, or materials needed for that step.
3. Open **Image**.
4. Arrange the Fusion viewport for the instruction. Hide/show components, use Fusion visibility states, highlight/select geometry, ghost items, or otherwise prepare the view that should appear in the guide.
5. Select **Capture View**. SAGA captures the prepared viewport and advances to **Markup**.
6. In **Markup**, enter the written instruction.
7. Add any notices and click **Add Notice** for each notice you want to keep.
8. Add any visual markup that improves the image.
9. Select **Apply Markup to Step**.

`Apply Markup to Step` is the point that applies the current instruction/markup state to the step for publication. Markup remains editable in the saved project.

### Notice placement

SAGA places notice types automatically:

- **Above the instruction:** Do not, Warning, Caution.
- **Below the instruction:** Information, Inspect, Check.

More than one notice may be added. Existing notices may be reordered or deleted.

### Markup tools

| Tool | Purpose |
|---|---|
| **Select** | Select and edit existing markup; move an item, move endpoints where applicable, duplicate, change layer order, or delete it. |
| **Arrow** | Directional pointer. First click sets the start; second click sets the destination/object being indicated. |
| **Leader** | Non-directional connector line. It may be solid or dashed. |
| **Alignment** | Dashed visual alignment aid used to show alignment between parts. |
| **Label** | Places entered label text at the clicked location; Select may move it afterward. |
| **Part Callout** | BOM-aware part identification with quantity/BOM-effect options and an optional movable leader. |
| **Marker** | Visual symbol for parts, processes, or non-BOM actions such as glue or cut. |

### Part Callout BOM effect

- **Install or use quantity** consumes/allocates the displayed quantity against the catalog total.
- **Reference only** identifies the item without consuming another unit.

With **Part callout leader** enabled, the callout has a movable leader. Without it, the callout is a standalone bubble.

## Configuration paths

Create the normal shared step first, including capture and markup. Then:

1. Return to **Details** on the last shared step before the alternatives begin.
2. Select **Create Split Here**.
3. Name the primary path and the alternate path. The primary path defaults to `Standard` when the split comes from the main sequence; when splitting from an existing branch, the current branch name is used as that path context.
4. Select **Create Split**.

The split may be created as a placeholder. You can keep authoring the main path and return to the alternate path later.

To author a branch:

1. Open the Step view/path control and select **Manage**.
2. In Configuration paths, find the path you want and select **View**.
3. Confirm that Step view shows the intended branch.
4. Select **+ New [Branch name] Step**.
5. Author the branch step with the same Details → Image → Markup → Apply Markup workflow used for an ordinary step.

To return to the main path, use Manage/View again and select the main path.

SAGA numbers branch steps automatically. For a split after Step 1, examples are:

- first step of the first alternate branch: `1B.1`;
- second step in that branch: `1B.2`;
- first step in another branch from Step 1: `1C.1`.

The last step on the main path is the overall final step. The last step on a branch is the path-ending/final step for that branch. These indicators are derived automatically from step order; the author does not manually designate them.

## Save, Check Project, and PDF

When editing is complete:

1. Open **Project** and select **Save**.
2. Confirm the green **Saved** message.
3. Run **Check Project**.
4. Fix blocking errors. Review warnings; warnings do not stop PDF generation.
5. Open **PDF**.
6. Choose **US Letter** or **A4**.
7. Choose **Portrait** or **Landscape**.
8. Choose whether to include the Cover page, Contents and links, and Bill of materials.
9. Select **Generate PDF**.

SAGA reports that it is checking the project and generating the PDF. Large images may take longer. When generation succeeds, SAGA displays the created PDF's filename/location.

After a save, later Fusion navigation can cause SAGA to show `Unsaved` again because Fusion's internal view/timeline navigation has changed. The SAGA document content that was successfully saved remains saved. SAGA does not save unrelated Fusion model or viewport edits.

**Congratulations — you have created your first assembly guide with SAGA.**
