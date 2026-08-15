# SAGA for Fusion — User Guide Production Pass 01

This package converts the owner walkthrough into a controlled manual-production source set.

## Rules used

- Real SAGA/Fusion screenshots only.
- No UI was redrawn or regenerated.
- Personal Windows paths were blurred where selected images expose them.
- Private owner-build headers were cropped when they were not instructional.
- The release-only distinction is preserved: the public product is **SAGA**, not “SAGA Owner.”
- Owner annotations were retained only where they materially explain a control.
- The original raw screenshot is preserved in `selected_raw/` for every edited publication image.
- Handoff screenshot `26 - Marker Example for Glue.png` was confirmed to be exactly identical to the walkthrough source used for `13_markup_combined_example.png`.

## Important corrections identified for the current GitHub User Guide

1. **Instruction and notices are authored in Markup**, not in Details.
2. Markup tools are seven distinct controls: Select, Arrow, Leader, Alignment, Label, Part Callout, Marker.
3. Alignment is specifically a dashed visual alignment aid, not a generic leader.
4. Transparent background is OFF on the first run, then persists after the user selects it; it may still be toggled for an individual capture.
5. Item Category choices shown in the owner build are Part, Hardware, Tool, Consumable.
6. Part Callout BOM effect distinguishes quantity use/allocation from Reference only.
7. `Apply Markup to Step` is the commit point for the current instruction/markup state used for publication.
8. Configuration paths need the actual Manage/View workflow and automatic branch numbering (`1B.1`, `1B.2`, `1C.1`, etc.).
9. The last main-path step is the overall final step; the last step of a branch is that path end/final step. SAGA derives these automatically from order.
10. Save is on the Project tab. The green `Saved` indicator confirms the SAGA document was saved. Subsequent Fusion navigation can make the UI show `Unsaved` again because of Fusion view/timeline navigation; that does not mean the previously saved SAGA document content was lost. SAGA does not save unrelated Fusion model/viewport edits.
11. Check Project must clear blocking errors before publication; warnings are review items and do not block PDF generation.
12. PDF publication supports US Letter or A4, Portrait or Landscape, with Cover page, Contents and links, and Bill of materials options.
13. During generation SAGA reports that it is checking the project and generating the PDF; on success it displays the output filename/location.
14. Leaving Markup with unapplied work must preserve the documented Apply / Discard / Cancel consequences, including the previously observed recapture recovery case after Discard.

## GitHub staging

Recommended repository destination for the final images:

`assets/user-guide/`

Do not update `user-guide.md` to these filenames until the PNG files have been uploaded to the repository.
