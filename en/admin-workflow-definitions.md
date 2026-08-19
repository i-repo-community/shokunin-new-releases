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

## Good to know

- Different sites and different jobs can each have their own procedure — no coding required.
- When a definition is updated, subsequent reports use the new revision. Reports already in
  progress keep the version they were started on.
- The two buttons above appear **only for customers who have their own i-Reporter** — see "Who this applies to" above.
- Uploading an XML file by hand continues to work exactly as before.
