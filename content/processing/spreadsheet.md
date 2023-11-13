---
section: Processing Manual
nav_order: 2
title: ArchivesSpace Spreadsheet Template
---

Use the ArchiveSpace Spreadsheet Upload Template to create the metadata needed to build the collection's finding aid.  

Rather than beginning to work in the template, you'll want to make a copy by using "Save As" into the proper file location. 

To find the spreadsheet, follow this pile path: **Share Point > spec > Collections > Processed Collections > Finding Aid Files > choose the group you're adding to > add a folder with your collections identifier (ex: MG 571)**

{% capture text %}
**NOTE:** Fields in the spreadsheet template that are colored RED are required fields.
{% endcapture %}

{% include alert.html text=text color="danger" %}

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