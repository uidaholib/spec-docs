---
section: Processing Manual
nav_order: 4
title: AS Spreadsheet - Digital Materials
---

For born-digital and hybrid collections, some fields in the **[ArchiveSpace Template](https://vandalsuidaho.sharepoint.com/:x:/r/sites/Storage-Library/Documents/spec/Collections/Processed%20Collections/Finding%20Aid%20Files/AS_spreadsheet_template.xlsx?d=w4a88ebe4a32b4e72b3d05ceb320d7e6b&csf=1&web=1&e=bfs5fC)** can be filled in using information from the **DROID** spreadsheet created during the **[Digital Material Ingest]({{ '/content/processing/digital-ingest.html' | relative_url }})** procedures. 

Rather than beginning to work in the template, you'll want to make a copy by using **Save As** into the proper file location. To save properly, follow this pile path: *Share Point > spec > Collections > Processed Collections > Finding Aid Files > choose the group you're adding to > add a folder with your collections identifier (ex: MG 571)*

{% capture text %}
**NOTE:** Fields in the spreadsheet template that are colored RED are required fields.
{% endcapture %}

{% include alert.html text=text color="warning" %}

{% include figure.html img="template-example.jpg" alt="spreadsheet example" caption="" width="" %}

Below are basic notes on completing the spreadsheet. 

{:.table .table-bordered}
| Field | Required | Content | Examples |
| - | ----- | -------- | -------- |
| EAD ID | Yes | This is based on the ID. The formula is NTD+ID. | MG 571 would have an EAD ID of *NTDMG571*. |
| Title | Yes | This is the title of the series, sub-series, folder, or item. Name field text could be copied from DROID or index if available. | Series I: Personal papers; Sub-series I: College notes; Chemistry course notes |
| Hierarchical Relationship | Yes | This is how nesting is created within finding aid records. Generally the *Series* entry will be 1, the *sub-series* will be 2, and the *folder* will be 3. If no *sub-series*, then the *folder* will be 2. |
| Description Level | Yes | This is a controlled field and you must choose one of the preset options -- *Class, Collection, File, Fonds, Item, Other Level, Records Group, Series, Sub-Fonds, Sub-Group, Sub-Series*. The most common are Series, Sub-Series, and File. |

Example:
{% include figure.html img="ead-example-2.jpg" alt="spreadsheet example" caption="" width="" %}

{:.table .table-bordered}
| Field | Required | Content | Examples |
| - | ----- | -------- | -------- |
| Date (1) Label | Optional | If creation date of material is known, use *Creation*. If creation date unknown, use *Modified.* Modified date is when the digital material was last ingested or when material was made into a digital asset. It can also be pulled from DROID. If creation date and modified dates are known, fill out both Date (1) and Date (2) sections. |
| Date (1) Begin | Optional | Must be written in YYYY-MM-DD, YYYY-MM, or YYYY. Spreadsheet cell should be formatted as *text* to avoid issues. Can be copied from DROID field *LAST_MODIFIED.*  | 2023-02-06T15:12:54 (from DROID), remove timestamp so in AS spreadsheet: 2023-02-06 |
| Date (1) End | Optional | If there is a date range for the materials fill in both the begin date AND the end date fields. Must be written in YYYY-MM-DD, YYYY-MM, or YYYY. | Begin: 1995; End: 2006 |
| Date Type | Yes | If one date known, select *single*. If date range known, select *inclusive*. *Bulk* can be selected if most material comes from one date over another. | Materials are from 1955-1995, so *inclusive*. |
| Date Expression | Optional | If dates known, write them out here. | Date range is from 1995-01 to 1998-06, then written is January 1995 - June 1998; Date is 2008-09-15 then 15 September 2008. |
| Extent Portion | Optional | Generally this will be "whole" though "part" is also an option. | 
| Extent Number | Yes | Numerical expression of Megabytes, Gigabytes, or Terabytes. Note: DROID does size in bytes but AS doesn’t have this as a dropdown option. Use byte calculator or Excel formula =CELL/(1024*1024). |
| Extent type | Yes | Megabytes, Gigabytes, or Terabytes. Note: DROID does size in bytes but AS doesn’t have this as a dropdown option. Use byte calculator. |
| Container Summary | Optional | Number of files located in the digital folder. | 18 files, 2 folders |
| Physical Details | Optional | Copy *MIME_TYPE* from DROID, or type in the file type  | jpg files: image/tiff |
| Dimensions | Optional | Copy *FORMAT_NAME* from DROID, or type in the file format type. | Tagged Image File Format |
| Container Instance Type | Yes | This is often "Mixed Materials" for a general manuscript collection, but could also be Books, Audio, Computer Disks, Maps, Realia, Microform, etc.|
| Top Container Type | Yes | For digital collections, type *Object*. |
| Tope Container [indicator] | Yes | Type *Digital*. |
| Child Type | Optional | Type *Object* |
| Child indicator | Optional | Copy from the NAME field in DROID, or type file name with extension. | badluck51-01-color.tif |