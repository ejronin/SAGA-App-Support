---
layout: page
title: Troubleshooting
---

Use this page for common startup, project, publication, and Marketplace-access problems. For workflow details, see the [User Guide](user-guide.md).

## SAGA does not appear in Fusion

1. Close and reopen Fusion after installation.
2. Open **Utilities > Scripts and Add-Ins**.
3. Select the **Add-Ins** tab and look for **SAGA**.
4. Select SAGA and choose **Run**.

SAGA does not start automatically by default. Fusion may allow you to enable automatic startup later.

If SAGA is missing from the Add-Ins list, confirm that the Autodesk Marketplace installer completed successfully. Close Fusion and reinstall the current Marketplace package before trying again.

## SAGA starts, but its command is missing

Stop SAGA from **Scripts and Add-Ins**, start it again, and reopen the relevant Fusion workspace. Restart Fusion if the command is still missing.

## A project will not open

Check that:

- The complete SAGA project folder is still together.
- The project file was not renamed separately from its supporting folders.
- The folder is available and writable.
- Cloud-sync or network software has finished downloading the files.

When testing a damaged or incomplete project, work from a local copy and keep the original unchanged.

See [Projects and local storage](user-guide.md#projects-and-local-storage) for the expected project-folder behavior.

## A project will not save

Confirm that the project folder is not read-only, Windows has not blocked access to it, and enough disk space is available. Avoid protected Windows system folders.

## A captured image is wrong or outdated

Arrange the Fusion model again and replace the step capture. After editing markup, select **Apply Markup to Step** so the image used for publication is updated.

Replacing a capture also clears markup tied to the old image. See [Steps, captures, and markup](user-guide.md#steps-captures-and-markup) before replacing a capture you may still need.

## Markup appears in the editor but not in the PDF

Return to the step, select **Apply Markup to Step**, save the project, and generate the PDF again.

## The project check reports an error

Correct errors before publishing. Common causes include missing step images, incomplete required project information, invalid quantities, or missing files. Review warnings and leave them only when the result is intentional.

See [Check Project](user-guide.md#check-project) for the documented error and warning behavior.

## PDF generation fails

1. Run **Check Project** and correct all errors.
2. Confirm that the project folder is writable.
3. Confirm that referenced images still exist.
4. Close any existing PDF with the same output name.
5. Generate the PDF again.

Large projects and high-resolution images may take longer to process.

## A trial or purchase is not recognized

1. Confirm that Fusion is signed in to the same Autodesk account used for the Marketplace trial or purchase.
2. Confirm that the computer is online.
3. Return to SAGA and select **Check again**.
4. If access is still not recognized, close and restart Fusion, start SAGA again, and recheck access.

SAGA uses Autodesk Marketplace entitlement verification for both the Free 30-Day Trial and purchased access. SAGA does not run a separate local trial clock.

A previously successful Autodesk access result may be used for up to 24 hours when Autodesk's entitlement service is temporarily unavailable. A completed negative response from Autodesk takes effect immediately and is not overridden by the prior successful result.

Do not delete SAGA's local entitlement data unless support asks you to do so. Removing it requires online re-verification and does not reset, extend, or cancel a Marketplace trial or purchase.

See [Marketplace access](user-guide.md#marketplace-access) for the full access model.

## The trial or Marketplace access has ended

When Autodesk no longer reports valid Marketplace access, SAGA authoring and PDF publication remain unavailable until valid access is reported again.

Existing SAGA project folders and previously generated PDFs are not deleted or altered when access ends.

If you believe access should still be active, follow the steps in [A trial or purchase is not recognized](#a-trial-or-purchase-is-not-recognized).

## SAGA stopped unexpectedly

Restart Fusion and reopen the project. Do not overwrite the original project while investigating possible corruption.

When contacting support, include:

- SAGA version
- Fusion version
- Windows version
- The exact error message, when one appears
- Steps that reproduce the problem
- A screenshot or local SAGA log when useful

SAGA logs are stored under:

```text
%LOCALAPPDATA%\SAGA\logs
```

Remove confidential project information before sending logs or screenshots unless it is necessary to diagnose the issue.

## Uninstalling SAGA

Use Windows **Installed Apps** or the Autodesk-provided uninstall process. Close Fusion before uninstalling. Uninstalling SAGA should not delete user-created project folders or published PDFs.

## Contact support

Email **sagaappsupport@gmail.com**. See the [Support Policy](support.md) for covered issues and the information to include.
