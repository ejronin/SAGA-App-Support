---
layout: page
title: Troubleshooting
---

# Troubleshooting SAGA

## SAGA does not appear in Fusion

1. Close and reopen Fusion after installation.
2. Open **Utilities > Scripts and Add-Ins**.
3. Select the **Add-Ins** tab and look for **SAGA**.
4. Select SAGA and choose **Run**.

SAGA does not start automatically by default. Fusion may allow you to enable automatic startup later.

When SAGA is missing from the Add-Ins list, confirm that the Autodesk Marketplace installer completed successfully. Reinstall the current package before attempting a manual folder installation.

## SAGA starts, but its command is missing

Stop SAGA from **Scripts and Add-Ins**, start it again, and reopen the relevant Fusion workspace. Restart Fusion if the command is still missing.

## A project will not open

Check that:

- The complete SAGA project folder is still together
- The project file was not renamed separately from its supporting folders
- The folder is available and writable
- Cloud-sync or network software has finished downloading the files

When testing a damaged or incomplete project, work from a local copy and keep the original unchanged.

## A project will not save

Confirm that the project folder is not read-only, Windows has not blocked access to it, and enough disk space is available. Avoid protected Windows system folders.

## A captured image is wrong or outdated

Arrange the Fusion model again and replace the step capture. After editing markup, select **Apply Markup to Step** so the image used for publication is updated.

## Markup appears in the editor but not in the PDF

Return to the step, apply the markup to the step image, save the project, and generate the PDF again.

## The project check reports an error

Correct errors before publishing. Common causes include missing step images, incomplete required project information, invalid quantities, or missing files. Review warnings and leave them only when the result is intentional.

## PDF generation fails

1. Run **Check Project** and correct all errors.
2. Confirm that the project folder is writable.
3. Confirm that referenced images still exist.
4. Close any existing PDF with the same output name.
5. Generate the PDF again.

Large projects and high-resolution images may take longer to process.

## A purchase is not recognized

- Confirm that Fusion is signed into the Autodesk account used for the Marketplace purchase.
- Confirm that the computer is online.
- Close and restart Fusion, then start SAGA again.
- Check whether Autodesk Marketplace services are available.

A previously verified purchase may continue to work temporarily through SAGA's local entitlement cache. Do not delete local licensing data unless support asks you to do so.

## The evaluation has expired

Existing SAGA projects and previously generated files remain on the computer. Continued use requires a valid Autodesk Marketplace entitlement.

## SAGA stopped unexpectedly

Restart Fusion and reopen the project. Do not overwrite the original project while investigating possible corruption. Include the SAGA version, Fusion version, Windows version, exact error message, and steps that reproduce the problem when contacting support.

## Uninstalling SAGA

Use Windows **Installed Apps** or the Autodesk-provided uninstall process. Close Fusion before uninstalling. Uninstalling SAGA should not delete user-created project folders or published PDFs.

## Contact support

Email **sagaappsupport@gmail.com**. See the [Support Policy](support) for covered issues and the information to include.
