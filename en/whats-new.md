---
title: What's New
nav_order: 11
---

[🌐 日本語](../ja/whats-new.html)

# What's New

News about Shokunin.new features, improvements, and fixes.

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

### Fixes

- Fixed unselectable reports appearing in the "Azusa Advice" list and in the list shown when adding photos to an existing report. Both lists now show photo reports only. To add photos to a workflow report, use the "Add photos" button in the Report List.
- Amount fields now show the yen mark "¥" correctly.
- Choice labels that contain a comma (such as "5,700円") now display correctly.
- Tapping a choice now highlights only the option you tapped (fixed a case where similar options were highlighted together).
- On optional single-choice fields, tapping the selected option again now clears your answer (required fields keep their selection).

## 2026-07

### Improvements

- Added a "Steps" list to workflow forms. Search steps by name and tap to jump directly to any step; Review screen items are also tappable.

### Announcements

- The Shokunin.new public website is now open.
