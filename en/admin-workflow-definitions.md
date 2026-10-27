---
title: Workflow Definitions
parent: Supervisors (admin screen)
grand_parent: User Manual
nav_order: 6
---

[🌐 日本語](../ja/admin-workflow-definitions.html)

# Workflow Definitions

Define the reporting procedures ([workflows](screen-workflow.html)) craftsmen follow on-site, as forms.

## What you can do

- Define the items a report needs (text, photos, choices, and more) as ordered steps.
- Assemble the flow visually, including branches and guidance.
- Assign a defined workflow to craftsmen via [Dispatch Management](admin-dispatch.html).
- Review submitted workflow reports in [Report History](admin-report-history.html).

## Importing from i-Reporter and keeping definitions current

If you have your own i-Reporter, two buttons at the top of the screen let you manage
definitions without exporting XML from i-Reporter Designer and uploading it by hand.

### Who this applies to

Whether the two buttons appear depends on how you use Shokunin.new.

| How you use it | The two buttons | How report definitions are registered |
|---|---|---|
| **You have your own i-Reporter**<br>(your own i-Reporter contract, running in your own environment) | Shown | Import from the list, or upload XML — either way |
| **You do not have an i-Reporter account**<br>(you use the shared i-Reporter environment Shokunin.new provides) | Not shown | Upload the XML file, as before |

The shared i-Reporter environment is used by several customers at once, so the upload step is
kept in place to make sure each customer's report definitions stay separate. In both cases,
registering a definition by uploading XML works exactly as it always has.

### "Import from i-Reporter" — add forms SNEW does not have yet

Lists the published report definitions on your i-Reporter server. Tick the ones you want and
import them, and each becomes a new workflow.

- Definitions SNEW already has are grouped under "Already in SNEW" and **cannot be
  selected**. Importing never modifies an existing workflow.
- Only **published** definitions are listed. Anything still in Test status on the i-Reporter
  side does not appear.

### "Sync definitions" — bring existing forms up to date

Checks whether any definition SNEW already holds has been updated on the i-Reporter side and
pulls the latest version if so. It never creates a new workflow.

- Workflows with a newer version available are marked "**Update available**", and the button
  shows how many there are.
- Until you sync, craftsmen keep seeing the previous version of the steps.
- **Workflows whose XML you uploaded by hand do not show "Update available" until you run
  Sync definitions once.** Syncing records which version of the definition SNEW holds, and
  that record is what later changes are compared against — with no record, there is nothing
  to compare. We recommend syncing once after uploading. Workflows added with "Import from
  i-Reporter" are recorded at import time, so they are covered from the start.

## i-Reporter network settings

Networks set between fields in the i-Reporter form (locked, narrowed choices, required, value comparison, and so on) carry over to the craftsman's form (see [Workflows](screen-workflow.html)).

- When you upload an XML, the preview shows "… field links". A notice appears if the form uses network settings the web form doesn't apply (no-entry-needed mark, follower auto-fill, custom-master default search), or links that don't connect two fields.
- On the flow canvas, networks are shown as **purple dashed lines** with labels such as "🔒 Locked", "Narrows", "Required" or "≧". Tap or click a line or its label ("ⓘ" on links without a label) to see what the link does.
- The purple lines are read from the i-Reporter definition and are **read-only**: they can't be edited or deleted on the canvas and are not saved as part of the flow. To change them, edit the form in i-Reporter Designer.
- **Grey dashed lines** are links the web form doesn't apply (labelled "(not applied on web)"). When the preceding field can't be filled in the web form (actions such as biometrics, QR code scanning, photos and so on), the web form doesn't apply the restriction, so the following field never ends up unusable.
- "Hide networks" hides them ("Show networks" brings them back).

## Thumbnails on the LINE work start cards

When craftsmen send 「業務開始」 (work start) in the chat, workflows appear as cards with a thumbnail. The thumbnail is the first page of the i-Reporter form, and you can also see it on the workflow list and detail screens.

- "**Refresh thumbnails**" at the top of the list fetches all missing or outdated thumbnails from i-Reporter at once. When some are missing, the button shows how many.
- "Refresh thumbnail" on the detail screen re-fetches the thumbnail for that workflow only.
- Click a thumbnail to enlarge it.
- If a thumbnail hasn't been fetched yet, or is outdated after a form update, a placeholder image is shown instead (craftsmen never see an outdated thumbnail). Forms with no thumbnail in i-Reporter also show the placeholder.

## Good to know

- Different sites and different jobs can each have their own procedure — no coding required.
- When a definition is updated, subsequent reports use the new revision. Reports already in
  progress keep the version they were started on.
- The two buttons above appear **only for customers who have their own i-Reporter** — see "Who this applies to" above.
- Uploading an XML file by hand continues to work exactly as before.
