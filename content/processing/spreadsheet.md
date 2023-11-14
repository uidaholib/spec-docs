---
section: Processing Manual
nav_order: 3
title: ArchivesSpace Spreadsheet
---

<div class="text-center mb-2">
    <a href="#{{ 'Physical Collections' | slugify }}" class="btn btn-secondary my-2 mx-1">Physical Collections</a>
    <a href="#{{ 'Born-Digital and Hybrid Collections' | slugify }}" class="btn btn-secondary my-2 mx-1">Born-Digital and Hybrid Collections</a>
</div>

### Physical Collections

Use the ArchiveSpace Spreadsheet Upload Template to create the metadata needed to build the collection's finding aid. The template is located in **SharePoint > spec > Collections > Processed Collections > Finding Aid Files > [AS_spreadsheet_template.xlsx](https://vandalsuidaho.sharepoint.com/:x:/r/sites/Storage-Library/Documents/spec/Collections/Processed%20Collections/Finding%20Aid%20Files/AS_spreadsheet_template.xlsx?d=w4a88ebe4a32b4e72b3d05ceb320d7e6b&csf=1&web=1&e=bfs5fC)**

Rather than beginning to work in the template, you'll want to make a copy by using **Save As** into the proper file location. To save properly, follow this pile path: *Share Point > spec > Collections > Processed Collections > Finding Aid Files > choose the group you're adding to > add a folder with your collections identifier (ex: MG 571)*

{% capture text %}
**NOTE:** Fields in the spreadsheet template that are colored RED are required fields. This template is usually used for collections that are more than one box. Small collections can be added manually in ArchiveSpace.
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
| Extent Portion | Optional | Generally this will be "whole" though "part" is also an option. | 
| Extent Number | Yes | If Extent section filled, this is required. Numerical expression of material. | A folder contains 45 negatives: Extent Portion *whole*, Extent Number *45*. |
| Extent type | Yes | If Extent section filled, this is required. Frequently the type is "folder" and the extent is "1" when you are cataloging at the folder level. Other examples of extent types include items, cassettes, megabytes, photographic prints, reels, volumes, pages. |
| Physical Details | Optional | A brief description of materials. This will appear in the finding aid and helps researchers know if the folder contains something they might be looking for. Include details that assist with discovery but be succinct. | Files that are negatives and in bad condition: b&w negatives (poor condition) |
| Container Instance Type | Yes | This is often "Mixed Materials" for a general manuscript collection, but could also be Books, Audio, Computer Disks, Maps, Realia, Microform, etc.|
| Top Container Type | Yes | Generally this will be "Box," but could also be Drawer, Reel, Case, Frame, etc. |
| Tope Container [indicator] | Yes | This is the box (or drawer) number. |
| Child Type | Optional | Generally this will be "Folder," but could also be Carton, Reel, Frame, etc.|
| Child indicator | Optional | This is the folder number. Folders can be numbered in one of two ways: Every folder has a unique number, starting with 1 and going as high as needed, OR every box starts with folder 1. Whichever you choose, stay consistent through the collection. |

**This is all the basic information needed to create a container list in ArchivesSpace and thus a finding aid in Archives West. If there are digital objects that can be linked to the finding aid, use columns BA and BB. Note that digital object titles cannot have quotation marks.**

---
### Born-Digital and Hybrid Collections

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