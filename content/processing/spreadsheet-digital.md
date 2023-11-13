---
section: Processing Manual
nav_order: 5
title: AS Spreadsheet Template - Digital Materials
---

For born-digital and hybrid collections, some fields in the [ArchiveSpace Template](https://vandalsuidaho.sharepoint.com/:x:/r/sites/Storage-Library/Documents/spec/Collections/Processed%20Collections/Finding%20Aid%20Files/AS_spreadsheet_template.xlsx?d=w4a88ebe4a32b4e72b3d05ceb320d7e6b&csf=1&web=1&e=bfs5fC) can be filled in using information from the DROID spreadsheet created during the Digital Material Ingest Procedures. 

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
| Title | Yes | This is the title of the series, sub-series, folder, or item. In most cases, the first line of the spread sheet will be a series entry. | Series I: Personal papers; Sub-series I: College notes; Chemistry course notes |
| Hierarchical Relationship | Yes | This is how nesting is created within finding aid records. Generally the *Series* entry will be 1, the *sub-series* will be 2, and the *folder* will be 3. If no *sub-series*, then the *folder* will be 2. |
| Description Level | Yes | This is a controlled field and you must choose one of the preset options -- *Class, Collection, File, Fonds, Item, Other Level, Records Group, Series, Sub-Fonds, Sub-Group, Sub-Series*. The most common are Series, Sub-Series, and File. |

Example 1: 
{% include figure.html img="ead-example.jpg" alt="spreadsheet example" caption="" width="" %}
---
Example 2:
{% include figure.html img="ead-example-2.jpg" alt="spreadsheet example" caption="" width="" %}

{:.table .table-bordered}
| Field | Required | Content | Examples |
| - | ----- | -------- | -------- |
| Date Label | Optional | Usually creation date of materials is selected. Type *Creation.*  A brochure from 1995 4-H conference, label is *Creation*. |
| Date Begin | Optional | Must be written in YYYY-MM-DD, YYYY-MM, or YYYY. Spreadsheet cell should be formatted as *text* to avoid issues. | 1995-05-18  ; 1987-04 ; 2006 |
| Date End | Optional | If there is a date range for the materials fill in both the begin date AND the end date fields. Must be written in YYYY-MM-DD, YYYY-MM, or YYYY. | Begin: 1995; End: 2006 |
| Date Type | Yes | If one date known, select *single*. If date range known, select *inclusive*. *Bulk* can be selected if most material comes from one date over another. | Materials are from 1955-1995, so *inclusive*. |
| Date Expression | Optional | If dates known, write them out here. | Date range is from 1995-01 to 1998-06, then written is January 1995 - June 1998; Date is 2008-09-15 then 15 September 2008. |