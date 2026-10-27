---
title: Workflows
parent: Craftsmen (LINE)
grand_parent: User Manual
nav_order: 5
---

[🌐 日本語](../ja/screen-workflow.html)

# Workflows

Workflows let you **report along a defined procedure**. You fill in the steps your supervisor defined as a form, so nothing gets missed.

## How it works

1. Tap "Start work" in the rich menu (Work reports tab), or send 「業務開始」 or "Start work" in the chat, and the workflows you can use arrive as **cards**. Each card shows a thumbnail of the form's first page, so you can pick one at a glance (the most recently updated workflows come first).
2. Tap "**Start**" on the card you want. After a short "Preparing the form…" message, the form opens directly.
3. Follow the on-screen steps, adding photos and information at each one.
4. Finish all steps and submit — a report is created.

- Workflows assigned to you through Dispatch Management still start from the "work start" card in the dispatch notification, as before.
- If the form can't be opened, tap "Try again".

## Switching views (One at a time / By sheet)

For every workflow, a switch at the top of the form changes how it is shown. A workflow without a flow (step order) set up goes through the form's fields one at a time, in form order.

- **One at a time**: one field per screen, following the guidance and the Yes/No branches.
- **By sheet**: all fields of each form sheet together — handy when you want to see everything while you fill it in.

Whatever you enter in one view carries over to the other. The view you chose last is used the next time you open a form (until you choose, a workflow with a flow set up opens One at a time, others By sheet).

In the By sheet view:

- Branch questions (Yes / No) appear in their place in the step order (right below the field before them), and you can answer them right there. Once you answer, the related fields appear straight away. You can also change an answer by tapping Yes or No again.
- Fields you don't need to fill because of a branch answer are grayed out as "**Not needed for your answers**" (nothing to enter, and they are not submitted).
- Fields behind a branch question you haven't answered yet show "Shown after you answer “(question)”". They appear once you answer that question.
- Once every question is answered, you can submit from the By sheet view. If an answer (or an entered value) ends the flow, a message says so, and you can't submit until you change that answer or field.

## Step list (jump navigation)

The "Steps" button at the top of the form opens a list of all steps.

- Search by step name and tap to jump directly to that step (Back/Next then work as usual).
- Steps on a branch arm you haven't selected are grayed out; they become available once that branch is selected.
- On the Review screen, tapping an item also jumps directly to that step.

## Asking Azusa

If the AI assistant Azusa's icon appears next to a field, tap the icon to ask Azusa about it ("Tap the icon to ask Azusa" is shown under the icon).

- You can ask about the field you tapped. The top of the chat shows "About (field name)", and Azusa answers about that field first, while also taking the rest of your form into account.
- Azusa only gives advice — she never fills in a field for you. You enter the values yourself.
- If you reopen the chat from another field's icon, a divider appears in the chat and the conversation switches to that field.
- Azusa's icon is shown in the One at a time view.

## Linked fields (networks)

When fields are linked by a network in the i-Reporter form, the web form behaves the same way.

| Link | What happens in the form |
|---|---|
| Locked | The field can't be filled until the field before it is. It shows 🔒 "Available after you fill in “…”". Clearing the earlier field also clears the linked field. |
| Warn | Filling it while the earlier field is empty asks "Prior item is not entered. Are you sure to continue entering?" |
| Narrowed choices | Only the options that match your choice in the earlier field are shown. If none match, it says "No options match what you chose in “…”". |
| Becomes required | Choosing a certain value in the earlier field makes this field required (*). |
| Value comparison | If the field must be, for example, greater than or at least the earlier field, a value that breaks the rule shows "(relation error)" and the report can't be submitted. |

- Once the earlier field is filled and the restriction is lifted, the field shows 🔗 "Linked with “…”", so you can see it's connected. "Narrowed" appears while its choices are narrowed, and "Required" while it's required.
- The step list shows the same: 🔒 (⚠ for warn) on fields that are held back, 🔗 on linked fields.
- In the by-sheet view, entering a field moves you on to the linked next field automatically.

## Kinds of fields you can fill

Beyond photos and text, forms can include several other kinds of fields (which ones appear depends on what your supervisor defined).

- **Toggle select (トグル選択)**: pick one option from round buttons. On optional fields, tapping the selected option again clears your answer.
- **Toggle total (トグル集計)**: automatically shows the total score of your toggle selections.
- **Time calculation (時刻計算)**: automatically calculates the difference between the times you enter (such as a duration).
- **Free draw / handwriting (自由描画)**: draw freehand with a pen. You can draw, erase, undo, and clear all — and reopen a saved report to keep editing your drawing.
- **Master select (マスター選択)**: pick from registered data (a master). Tap the box to see the list and choose from it; type part of a value to narrow it down (a hint under the box shows which item is searched, and an example once the list has loaded). If nothing matches, tap "Show list" to go back to the list; "Close list" closes it.

## Good to know

- The steps and fields are defined by your supervisor in the admin screen (Workflow Definitions), so they differ per site and per job.
- The resulting report appears in "Workflow reports" in the rich menu (see [Report List](screen-report-list.html)) and works like any other photo report — you can edit and download it the same way.
