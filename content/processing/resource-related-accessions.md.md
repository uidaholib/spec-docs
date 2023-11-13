---
section: Processing Manual
nav_order: 10
title: Resource Record - Related Accessions
topics: 
---

The **Finding Aid Data** section in the Resource Record houses finding aid creation information. 

{:.table .table-bordered}
| Field | Required | Content | Examples |
| - | ----- | -------- | -------- |
| EAD ID | Yes | This is based on the ID. The formula is NTD+ID. | MG 571 would have an EAD ID of *NTDMG571*. |
| EAD Location | Yes | Retrieve from [Archives West Management Tools](https://archiveswest.orbiscascade.org/tools/login.php?redirect=/tools/) site by clicking **ARK Request**, and requesting an ARK number. | 80444/xv147063

{% include figure.html img="ark.jpg" alt="ARK request example" caption="" width="60%" %}

{:.table .table-bordered}
| Field | Required | Content | Examples |
| - | ----- | -------- | -------- |
| Finding Aid Title | Yes | Guide to [Collection Title] | Guide to University of Idaho photograph collection |
| Finding Aid Subtitle | Optional | Not require nor a field used often. |
| Finding Aid Filing Title | Yes | Usually just the collection title. If a title with a person's name, the format is Last Name (First and Middle). | Vandal (Jane J.) papers |
| Finding Aid Date | Yes | Year the finding aid was completed. If a finding aid was updated, note the date of update in the Finding Aid Author field. | 2037 |
| Finding Aid Author | Yes | Finding Aid prepared by [name of person who prepared the finding aid] | Finding aid prepared by Jane Vandal; Finding aid prepared by Jane Vandal, updated by Joe Vandal in 2035. |
| Description Rules | Yes | Autopopulates as Describing Archives: A Content Standard (DACS) |
| Language of Description | Yes | Usually English. Include all languages found in the finding aid. | English; Spanish |
| Script of Description | Yes | Usually Latin. |
| Language of Description Note | Yes | Finding aid written in [whatever the language it is written in.] | Finding aid written in English. |
| Sponsor | Optional | If work on the collection is funded through a grant or other sponsor, make note of that. | Funding for encoding this finding aid was provided through a grant awarded by the National Endowment for the Humanities. |
| Edition Statement | Optional | For recording information about the edition of the finding aid. |
| Series Statement | Optional | Indicates any bibliographic series to which the finding aid belongs. |
| Finding Aid Status | Yes | When ready to upload to Archives West, mark as *Complete.* |
