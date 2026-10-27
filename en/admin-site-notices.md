---
title: Site Notices
parent: Supervisors (admin screen)
grand_parent: User Manual
nav_order: 9
---

[🌐 日本語](../ja/admin-site-notices.html)

# Site Notices

Register site details and prepare the construction business permit notice, workers’ accident insurance establishment notice, emergency contacts, and photo-report QR poster.

## Create or select a site

1. Open **Site Notices** in the admin screen.
   - To start a new site, choose **Create notices**. In the **Create a new site** form, enter the site name (required) and, if you know them, the construction number and address, then choose **Create**. Nothing is saved until you choose **Create**; **Cancel** creates nothing.
   - To continue a site you already saved, choose **Open a saved site** and select it from the list, or search for it. If no site matches your search, **Create a site named after your search** opens the same form with your search text as the site name.
   - To start from a past report, choose **Import site details from past reports**, select a site, and choose **Create notices for this site**. The form is filled in from the report; review the details, enter a site name if the report has none, and choose **Create**.
2. Enter the remaining site details in each form.
3. Maintain shared company details in **Company Profile**. Choose **Apply company profile** to copy them into the site forms. You can then edit permit details for each site.
4. Choose **Save** to save a draft. You can save even when some fields are incomplete.

Unsaved edits are identified on screen. If a confirmation appears when you switch sites or return to the list, save first or choose to discard the changes. If another user saved changes first, the page reports a conflict. Review your edits before reloading the latest saved version.

## Edit the forms

Choose a form from the left side and enter its details. The permit notice supports multiple general and special permits, industry categories, and engineer classifications. Enter the workers’ compensation insurance business operator’s address, name, and representative on the insurance form. This is separate from the company on the permit notice. Selecting fixed-term or continuous business changes the available business-period fields.

You can enter emergency contacts manually. A SYSTEM_ADMIN can import a prefecture’s designated-facility list (Saitama or Shizuoka) and public Medical Information Net data so users can search candidates by facility name, address, phone, or department. Each import is held for review and is used only after a SYSTEM_ADMIN checks and activates it. The hospital list is shared by all companies, with one active list per prefecture. The search uses the prefecture at the start of the site address; if the address names neither prefecture, choose one of the prefectures that has data. The initial dataset makes only 257 of 1,726 designation rows searchable because those are the rows with a unique match. A missing candidate does not mean a facility is undesignated, unregistered, or unable to accept emergency patients; enter contacts manually when needed. After copying a candidate, verify the facility-information date, workers’ compensation designation source and designated-list reference date, and emergency-patient acceptance status and confirmation date separately. Acceptance is never inferred automatically. If the candidate search itself fails, the page shows an error and HTTP status, separate from a no-candidate result. Search again manually after the connection recovers; contacts can still be entered manually.

Enter site coordinates manually or choose **Get current location**. Review the address and map position, then explicitly select the confirmation checkbox before saving. A medical facility’s coordinates are never copied to the worksite automatically.

You can create a **Draft PDF preview** at any time, without saving or completing the form. It uses the current unsaved edits and does not save site data. Every page is marked **Draft — includes unsaved edits**. If no forms are selected for export, the preview includes only the form currently open. Long content continues onto additional A3 form or A4 QR pages. Long QR information continues onto A4 pages as well. If the QR payload exceeds the code’s capacity, the code is not generated; the PDF explains why and points to the continuation pages. The entered values are unchanged.

**Final PDF** and **Excel** export saved forms that meet their required fields. If a selected form is incomplete or exceeds its printable capacity, the page identifies the affected field and explains what to correct; the emergency form instead continues onto additional pages without shrinking its text. Save unsaved changes before producing the final PDF or Excel. Creating a draft preview does not change saved data or its version. Each site keeps only its latest Final PDF: creating a new one replaces the previous one. For a site created from a photo report, admins can open the latest Final PDF in **Report history**: open that report, then the **Detail** tab. For a site created without a report, the Final PDF is shown in the preview, where you can download it.

In the final-export error list, select a missing field to switch to its form. To review the current layout without correcting the missing fields first, choose **Preview draft without correcting fields** in that list.

## Export PDF or Excel

1. Select the forms you need under **Forms to export**. Multiple selected forms are combined in one file. Select the photo-report QR when needed.
2. Choose **Draft PDF preview** to review work in progress. To create a posted **Final PDF** or **Excel** file, save your edits and complete the required fields first. Save any unsaved changes before final export.
3. Check the paper size and scale before printing. The permit, insurance, and emergency forms default to A3 landscape; the QR poster defaults to A4 portrait. Print the PDF at **Actual size** or 100%. Scaling changes the frame dimensions.

The emergency form prints a 56 pt title and labels and values of at least 42 pt. Long contacts and notes continue onto additional pages. Excel also prints at 100% without shrinking text; each continuation page repeats its contact identifier, so a form with many contacts can use several pages.

Form titles are printed in Japanese. The photo-report QR poster contains separate codes for the existing photo-report link and for adding the service as a friend.

The PDF frame targets 370 × 260 mm. In the October 2026 test environment, converting the Excel file to PDF with LibreOffice produced three A3 landscape frames measuring approximately 360 × 253.8 mm, 360 × 255.7 mm, and 360 × 255.5 mm. Paper, spreadsheet software, and printer settings can change dimensions or page breaks. After printing the permit and insurance forms, measure each frame and confirm it is at least 350 mm wide and 250 mm high. This minimum does not apply to the emergency contact form. If you edit the Excel file and then make a PDF, export it from your spreadsheet application and check the paper size, scale, and page count.

The screen, PDF, and Excel files were checked digitally. Printing on a physical printer and scanning the QR codes with a smartphone have not been tested. Review the output before posting it at a site.
