---
section: Processing Manual
nav_order: 5
title: Resource Record
---

The following are sections and fields a processor must fill out in order to have a complete Resource Record in ArchivesSpace. Use the information from your [Collection Description]({{ '/content/processing/collection-description.html' | relative_url }}) document to help fill out fields.

### 1. Log into [ArchivesSpace (AS)](https://uidaho.libraryhost.com/admin) & Create a Resource Record
- URL: [https://uidaho.libraryhost.com/admin](https://uidaho.libraryhost.com/admin).
- The username and password are established upon account creation.
- Create a Resource Record
    - Option 1:
        - If the collection has a previous Accession Record, find it by searching in ArchivesSpace. 
        - When found click "view" to view the record. Once at the record viewer window, in upper right hand corner select **Spawn**.
        - Click on *Resource*.
        - This will create a Resource Record using some of the information filled from the Accession Record.
    - Option 2:
        - In ArchivesSpace, click **Create** located next to the search box.
        - From the drop-down menu, click **Resource**.

---
### 2. Basic Information Fields 
The fields listed below should be filled for each resource record. Fields marked with * are mandatory (if information is known). Please consult with department colleagues if questions arise.

{:.table .table-bordered}
| Field | Required | Content | Examples |
| - | ----- | -------- | -------- |
| Title | Yes | The title will likely be the same unique name given to the donation. The name of the person/group + type of records, such as papers, records, or collection. | Joe Vandal papers |
| Identifier | Yes | Assign the identifier based on the next available number in the [List of All Collections](https://vandalsuidaho.sharepoint.com/:x:/r/sites/Storage-Library/Documents/spec/Collections/Processed%20Collections/List%20of%20All%20Processed%20Collections.xlsx?d=w5ab19cc4fbee525e912b7bcd8afa738a&csf=1&web=1&e=cs00Gc&nav=MTVfezAwMDAwMDAwLTAwMDEtMDAwMC0wMjAwLTAwMDAwMDAwMDAwMH0). If you have questions about the difference between MGs, UGs, and PGs, see the [Scope of Collections]({{ '/content/introduction/scope.html' | relative_url }}) documentation. |
| Level of Description | Yes | Drop-down menu. Usually *Collection*. |
| Resource Type | Optional | Drop-down menu. Best practice is to select the type even if this field isn't required in AS. Selections are *Collection, Publications, Records* and *Papers*. | University of Idaho photograph collection; Joe Vandal papers; Sunshine Mine Company records |
| Publish? | Optional | Check for to publish. |
| Restrictions Apply? | Optional | Check is there are restrictions. |
| Repository Processing Note | Optional | Not included in any reports or exports. Include additional processing information. |

---
### 3. Languages

The fields listed below should be filled for each resource record. Fields marked with * are mandatory (if information is known). Please consult with department colleagues if questions arise.

{:.table .table-bordered}
| Field | Required | Content | Examples |
| - | ----- | -------- | -------- |
| Language | Yes | The language term and code represented in the material(s) described. | English |
| Script | Optional | The script term and code represented in the material(s) described. | Latin |

---
### 4. Dates

The **Dates** section in the Resource Record is used to document the dates of the materials in the accession. Include both bulk and inclusive dates when appropriate. May already be filled in if spawned from Accession Record. Fields marked with * are mandatory (if information is known). Please consult with department colleagues if questions arise.

{:.table .table-bordered}
| Field | Required | Content | Examples |
| - | ----- | -------- | -------- |
| Label | Yes | Select what the date type is from this drop-down menu. Generally, **Creation** is selected. Consult a colleague if you think it should be something different. | Creation; Modified; Digitized |
| Expression | Yes | This field shows the dates that are visible in the accession record. More descriptive information can be included in this field, such as *circa.* | 1942-1987; circa 1985; 05 June 1947 |
| Type | Yes | Select *inclusive, bulk dates,* or *single* from drop-down menu. | **Inclusive** = dates encompass whole collection; **Bulk** = majority of materials are between two dates; **Single** = for material that only covers one date |
| Begin Date | Yes | First date in date range (yyyy-mm-dd). | May 25, 1947 would be 1947-05-25 |
| End Date | Yes | Last date in date range (yyyy-mm-dd). |
| Certainty | Optional | Are these circa dates? If so, choose ‘Approximate.’ If not leave blank. |

**Era** and **Calendar** autopopulates as *CE* and *Gregorian* respectively, generally no need to adjust. 

---
### 5. Extents

The **Extents** section in the Resource Record refers to the size of the collection (usually # of cubic feet, i.e. # of storage boxes). May already be filled in if spawned from an Accession Record.

{:.table .table-bordered}
| Field | Required | Content | Examples |
| - | ----- | -------- | -------- |
| Portion* | Yes | Normally, **Whole** is chosen because it describes entire collection. However, **Part** can be chosen is there are varying extents. If you are portioning in parts, you’ll need to add new sections for each portion using the “+” at the bottom of the section. | Physical or born-digital collection without variations = *Whole*; Hybrid collection with analog materials in boxes and assets on a USB drive = 2 *Part* sections |
| Number* | Yes | The numeric value of the extent. | Physical collection = *Whole, 5 (cubic feet)*; Hybrid collection = *Part, 2 (c.f.)* & *Part, 15 (megabytes)* |
| Type* | Yes | How the space is being accounted for. For digital collections it may be Megabytes, Gigabytes, or Terabytes. | Physical collection = *Whole, 5, cubic feet*; Born-Digital collection = *Whole, 5, gigabytes* | 
| Container Summary | Optional | Use this field to track number of boxes and as a guide to see if boxes are missing from a shelf. | 4 folders, 1 box
| Physical Details | Optional | Other physical details of the materials described. | Analog; b&w; negatives
| Dimensions | Optional | Dimensions of the materials described. | 29 cm; 7 in. |

---
### 6. Finding Aid Data

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

---
### 7. Related Accessions

The **Related Accessions** section in the Resource Record is sed for linking associated Accessions with the Resource. 

To link an accession:
1. Click *Add Related Accession*.
2. In the search bar, type in the accession id OR select *Browse* from the drop-down menu.
3. Once accession found, select to link.

Multiple accessions can be added. 

{% include figure.html img="accessions.jpg" alt="adding accessions" caption="" width="" %}

---
### 8. Agent Links 

The **Agent Links** associates the creator of the material with the record. It also links the source of material or subject of the materials described to provide information about their context.

To link an agent:
1. Click *Add Agent Link*.
2. In the **Role** dropdown menu select either *Creator, Source,* or *Subject*.
3. The **Relator** section narrows down the specifics of the creator, source, or subject. If unknown, skip.
4. In the **Agents** search bar, type in the entity you are trying to link.
    - If agent not found by searching, from the dropdown select *Browse*.
    - If agent not found in the system at all, hover over *Create* and select the type of agent you are linking.

##### Creating an Agent
- Search the [Library of Congress Name Authority File (LCNAF)](https://id.loc.gov/authorities/names.html) database to see if your agent has a LCNAF record.
    - If correct agent record populates, click on to view the full record.
        - This page will show accepted variants and the LCNAF Identifier (at the end of the URI link).
        - Use this information to fill out the fields when creating an agent in ArchivesSpace.

Example:
{% include figure.html img="name-result.jpg" alt="lcnaf name result" caption="" width="80%" %}
---
{% include figure.html img="record-page.jpg" alt="lcnaf name result" caption="" width="80%" %}
---

- After hovering over *Create* and selecting the type of agent you are linking:
    - The *Create Agent* window pops up. Check the **Publish?** box. Then scroll to the *Name Forms* section.
    - Fill in the following fields:

{:.table .table-bordered}
| Field | Required | Content | Examples |
| - | ----- | -------- | -------- |
| Authority ID | Yes (if known) | This is the LCNAF Identifier. | no2006026875 |
| Source | Yes | Select correct source from dropdown menu. | If from LCNAF, select *Library of Congress Name Authority File.* If source unknown, select *Unspecific ingested source*. |
| Rules | Yes | Information can be inferred from Source. | Usually select *Describing Archives: A Content Standard.* |
| Name Order | Yes | Autopopulates as *Indirect*. Usually leave as is. |
| Prefix | Optional | If there is a name prefix, include here. | Mrs. |
| Title | Optional | If title is part of a name, add here. | *Sir* (for Churchill, Winston, Sir, 1874-1965) |
| Primary Part of Name | Yes | Usually last name or surname of a person. | *Churchill* (for Churchill, Winston, Sir, 1874-1965) |
| Rest of Name | Yes (if known) | Include the rest of the entity's name. | *Winston* (for Churchill, Winston, Sir, 1874-1965) |
| Suffix | Optional | Term following a name that qualifies the name but is not a title. | *Jr.* |
| Fuller Form | Optional | The fuller form of first and middle names, when abbreviated. | *Hilda Doolittle* (for H.D., Hilda Doolittle, 1886-1961) |
| Number | Optional | A number, sometimes with a term, that qualifies the name. | *II* (for John Paul II) |
| Dates | Optional | Dates of existence for the named entity (i.e. birth and death year) | *1886-1961* (for H.D., Hilda Doolittle, 1886-1961) |

- Leave the rest of the fields blank, and click the blue **Create and Link to Agent** button. Process is complete.

{% capture text %}
**NOTE:** Multiple agent links can be added. 
{% endcapture %}

{% include alert.html text=text color="warning" %}
---
### 9. Subjects

The **Subjects** section in the Resource Record is used for linking Subjects with the materials described.

To add a subject: 
1. Click **Add Subject**.
2. In the *Subjects* search bar:
- Type to search for a subject already in ArchivesSpace
- Use the dropdown menu to *Browse* for subjects.
- Use the dropdown menu to *Create* a subject.

##### Creating a Subject
- Search the [Library of Congress Subject Headings (LCSH)](https://id.loc.gov/authorities/subjects.html) database to see if a subject has a LCSH record.
    - If correct subject record populates, click on to view the full record.
        - This page will show accepted variants and the LCSH Identifier (at the end of the URI link).
        - Use this information to fill out the fields when creating an agent in ArchivesSpace.

Example:
{% include figure.html img="subject-result.jpg" alt="lcsh name result" caption="" width="80%" %}

- After clicking *Create*, the *Create Subject* window pops up.
- Fill in the following fields:

{:.table .table-bordered}
| Field | Required | Content | Examples |
| - | ----- | -------- | -------- |
| Authority ID | Yes (if known) | This is the LCSH Identifier. | sh85148615 |
| Source | Yes | Select correct source from dropdown menu. | If from LCSH, select *Library of Congress Subject Headings.* If source unknown, select *Unspecific ingested source*. |
| Scope Note | Optional | Usually left blank. Explains what is meant/not meant in the definition of the term and in its use as a subject heading. |
| Term | Yes | Type in the term. | Wrestling |
| Type | Yes | Usually *Topical, Geographical,* or *Uniform Title*. Choose the correct type from the dropdown menu. |

- Leave the rest of the sections blank, and click the blue **Create and Link to Subject** button. Process is complete.

{% capture text %}
**NOTE:** Be sure to add three or more subjects. One MUST be a subject by Archives West. Consult colleagues for more information.
{% endcapture %}

{% include alert.html text=text color="warning" %}

---
### 10. Notes

This section adds additional descriptive information about the materials described, usually in the form of text or structured lists. Use the information from your [Collection Description]({{ '/content/processing/collection-description.html' | relative_url }}) document to help fill out fields.

To add a note:
1. Click *Add Note*.
2. Begin adding Note Types from the dropdown menu. Add as many as you can to provide researchers with as much collection information as possible.

{% capture text %}
**NOTE:** To link webpages, type <extref linktype="simple" title="webpage" actuate="onrequest" show="new" href="paste link here">"Samuel H. Hays," Idaho Statesman, undated.</extref>.
{% endcapture %}

{% include alert.html text=text color="warning" %}

Below are fields normally filled out by processors.

{:.table .table-bordered}
| Note Type | Content | Examples |
| - | -------- | -------- |
| Abstract | 2-3 sentence description of the collection. Will serve as the *Summary* section on [Archives West](https://archiveswest.orbiscascade.org/search.php?r=idu). | Records of the University of Idaho Press. |
| Arrangement | Include how the collection has been arranged. | Born-digital materials were made into a stand-alone series. Original order retained. |
| Bibliography | Include a bibliography if outside research done and compiled to complete the Biographical/Historical Note. |
| Bibliographical / Historical | Include historical context or biographical context about the collection. See [Composing a Collection Description]({{ '/content/processing/collection-description.html' | relative_url }}) to help fill out this field. |
| Conditions Governing Access | Inform researchers about accessing physical and digital materials. | Usually type: "Collection is open for research." |
| Conditions Governing Use | 