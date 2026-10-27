---
title: What's New
nav_order: 11
---

[🌐 日本語](../ja/whats-new.html)

# What's New

News about Shokunin.new features, improvements, and fixes.

## 2026-10

### New features

- **Create site notices in one place**: From **Site Notices** in the admin screen, prepare a construction business permit notice, workers’ compensation insurance establishment notice, building confirmation notice, emergency contacts, and a photo-report QR poster for each site. Review a PDF preview, then export PDF or Excel ([Site Notices](admin-site-notices.html)).
- **Turn a workflow report into a site poster**: Import steps from a past workflow report, edit step names, descriptions, cautions, and owners, then print the result. Long workflows can be arranged into up to eight poster steps ([Site Notices](admin-site-notices.html)).
- **Open saved site-notice PDFs from report details**: Admins can view or download the latest PDF saved for a site in **Report history** (open the photo report, then the **Detail** tab). Creating a new Final PDF replaces the previous one.

- **Your signature is now printed on the photo report PDF**: when you tap "Sign & complete" on the download screen, your signature is printed in the "作業コメント" (work comment) box on page 2 of the photo report PDF. It is printed while pending admin approval too; re-signing replaces it, and it is removed if an admin rejects or deletes it. Reports signed before this change get the signature the next time the report is updated ([Download](screen-download.html)).

- **The rich menu now has tabs**: "Photo reports", "Work reports" and "Help" group the buttons by task. Report lists are split into "Photo reports" and "Workflow reports", and "Project info form" is now "New report". If your LINE is set to a language other than Japanese, you see an English menu ([Registration & Profile](screen-registration.html)).

### Improvements

- **"Updating PDF…" while your signature is saved**: "Download PDF", email and share can't be tapped until saving finishes; then the latest PDF with your signature opens ([Download](screen-download.html)).
- **New button order in the rich menu**: on the Photo reports tab, "Azusa advice" and "Photo reports" have swapped places. The bottom row now reads, from left to right, "Azusa advice", "Photo reports" and "Project history" ([Registration & Profile](screen-registration.html)).

## 2026-09

### New features

- **Work start now shows cards**: when you send 「業務開始」 (work start) in the chat, workflows appear as cards with a thumbnail of the form. Tap "Start" and the form opens directly ([Workflows](screen-workflow.html)). You can also check and refresh the thumbnails in [Workflow Definitions](admin-workflow-definitions.html) on the admin screen.
- **Switch how the form is shown**: for workflows with a flow set up, you can switch between "One at a time" and "By sheet". What you enter carries over to both views. In the By sheet view you can also answer the Yes/No questions in place, and fields you don't need because of an answer are grayed out.
- Added **OpenAPI** under **System settings** in the admin sidebar. You can now check the specification of the API used for external system integrations directly from the admin screen. It appears only when you are signed in with an administrator account, and opens in a new tab.

### Improvements

- In workflow forms, "Tap the icon to ask Azusa" now appears under Azusa's icon. Azusa also now answers first about the field whose icon you tapped (the chat shows "About (field name)").
- In workflow forms, **master select** fields now show the list as soon as you tap the box, so you can pick without knowing a keyword. A hint under the box shows which item is searched (with an example once the list has loaded), and if nothing matches, "Show list" takes you back to the list.
- The list of access keys for external system integrations now **hides revoked and expired keys**. Only the keys you can currently use are shown, and a checkbox reveals the hidden ones. The keys themselves are never deleted, so the record of who created past reports with them is preserved.

### Fixes

- Fixed a problem where PDF generation could fail when several reports were created at almost the same time.
- Fixed a problem where the screen could keep waiting if i-Reporter stopped responding. It now stops after a set time and reports an error.
- Fixed a problem where edits to a report could be lost. If someone edited a report's comments or details while its PDF was being regenerated, that edit was sometimes not saved.
- Fixed a problem where a failed PDF generation also made the previous PDF unavailable. If a new PDF cannot be created, the existing one now stays in place.
- The update date printed on a report now reflects when the report's contents were last changed. Previously, regenerating the PDF without changing anything could move that date forward.

## 2026-08

### New

- Workflow forms now support more kinds of input fields.
  - **Toggle select (トグル選択)**: you can now fill in single-choice fields shown as round buttons.
  - **Toggle total (トグル集計)**: automatically shows the total score of your toggle selections.
  - **Time calculation (時刻計算)**: automatically calculates the difference between time fields (such as a duration).
- **Free draw / handwriting (自由描画)**: a new field you can draw on freehand with a pen. Draw, erase, undo, and clear all; you can also reopen a saved report and keep editing your drawing.
- **Import and sync report definitions from i-Reporter** (for customers who have their own i-Reporter; not shown if you do not have an i-Reporter account): the [Workflow Definitions](admin-workflow-definitions.html) screen can now list the report definitions on your i-Reporter server and import them directly. If a definition you already use is updated on the i-Reporter side, it is marked "Update available" and you can pull the latest version in one tap. Exporting XML files and uploading them by hand is no longer necessary — though manual upload still works as before. Note that workflows you uploaded by hand previously start showing "Update available" only after you have run Sync definitions once.

### Improvements

- Tapping "Next" now scrolls to the first empty required field for every kind of field (including toggle select and multi-select), not just text fields.
- The operation log can now be filtered by access-key events for external integrations ("API credential issued", "API credential rotated", "API credential revoked"). These entries appear only for customers using an external integration.

### Fixes

- Fixed unselectable reports appearing in the "Azusa Advice" list and in the list shown when adding photos to an existing report. Both lists now show photo reports only. To add photos to a workflow report, use the "Add photos" button in the Report List.
- Amount fields now show the yen mark "¥" correctly.
- Choice labels that contain a comma (such as "5,700円") now display correctly.
- Tapping a choice now highlights only the option you tapped (fixed a case where similar options were highlighted together).
- On optional single-choice fields, tapping the selected option again now clears your answer (required fields keep their selection).
- The report registration form keeps opening as usual after the LINE app change in October 2026.
- When the form opens with details such as the construction name or company name already filled in, values containing "?" or "+" are no longer cut short.
- Screens opened from LINE now still open, instead of showing an error, when part of the link is damaged.

## 2026-07

### Improvements

- Added a "Steps" list to workflow forms. Search steps by name and tap to jump directly to any step; Review screen items are also tappable.

### Announcements

- The Shokunin.new public website is now open.
