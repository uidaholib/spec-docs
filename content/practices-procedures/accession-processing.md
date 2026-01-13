---
section_id: Practices and Procedures
nav_order: 1
title: Accession and Processing Procedures
---
<div class="text-center mb-2">
    <a href="#{{ 'Accession Procedures' | slugify }}" class="btn btn-secondary my-2 mx-1">Accession Procedures</a>
    <a href="#{{ 'Processing Procedures' | slugify }}" class="btn btn-secondary my-2 mx-1">Processing Procedures</a>
    <a href="#{{ 'Born-Digital Accessioning and Processing' | slugify }}" class="btn btn-secondary my-2 mx-1">Born-Digital Accessioning and Processing</a>
</div>
---

### Accession Procedures

If materials are deemed appropriate for inclusion in Spec, they will be accessioned. Manuscript, university, or photograph collections that have been accessioned will be noted with an identifying number beginning with **MA** or **UA**. For a step-by-step guide to accessioning, see the **[Accession Manual]({{ '/content/accessions/rehouse.html' | relative_url }})**.

The following is a summary of steps which make up the accessioning process:  
1. If items cannot be accessioned immediately upon receipt, place items on shelving in intake area, as space allows, along with the completed Deed of Gift. 
2. Add an *accession* record to [ArchivesSpace (AS)](https://uidaho.libraryhost.com/admin) that includes donor and collection information, an accession number, and a preliminary inventory. 
3. Rehouse the materials if appropriate to condense for space saving or material stability. 
4. Assess how important the materials are to departmental priorities and make a note in the *[Prioritization Rating List](https://vandalsuidaho.sharepoint.com/:x:/r/sites/Storage-Library/Documents/spec/Departmental%20Projects/Processing%20Priorities%20Project/Prioritization%20Rating%20List%20-%20updated%20copy.xlsx?d=wb86306cdf2435792ab6e50c79276a8e2&csf=1&web=1&e=n20NdU)* (found in SharePoint). 
5. Find a temporary shelf location and note that in the AS accession record. 
6. Print **Accession Report** from AS and place in appropriate accession binder along with the Deed of Gift and/or any relevant communications. 
7. Work with department Head to ensure that a *thank-you* note is sent to the donor, when applicable (found in SharePoint). 

---
### Processing Procedures

Accessioned materials are made more useful and accessible through processing. Even a minimal level of processing should be the goal for all collections. While some collections may warrant a very thorough processing, box or folder-level descriptions should suffice in most instances. The level of detail should be determined by the complexity or variety of materials, the size of the collection, and a professional assessment of the collection's importance. This is a subjective process. For a step-by-step guide, see **[Processing Manual]({{ '/content/processing/collection-description.html' | relative_url }})**.  

The following is a summary of steps which should be used to process a collection:  

1. Create an inventory in an [AS spreadsheet template](https://vandalsuidaho.sharepoint.com/:x:/r/sites/Storage-Library/Documents/spec/Collections/Processed%20Collections/Finding%20Aid%20Files/AS_spreadsheet_template.xlsx?d=w4a88ebe4a32b4e72b3d05ceb320d7e6b&csf=1&web=1&e=w6sKLf) (found in SharePoint); the template will later be imported into [ArchivesSpace (AS)](https://uidaho.libraryhost.com/admin)
- If the collection is very small, it may be more efficient to work directly in AS 
2. Rehouse the collection (if not completed at time of accession) 
- Weed to remove personally sensitive or irrelevant materials, like financial receipts or medical records 
- Utilize acid-free housing materials
        - Guidance from the National Archives should be used when making decisions about rehousing materials[^1]
- Make a professional determination of the best order for collection 
        - Original order is preferred in the archival field 
        - If collection bares no evidence of imposed order from the creator, subject or chronological order may be appropriate 
3. Create summary, scope of contents, biographical/historical statements in AS 
4. Identify subject tags in AS 
5. Complete finding aid 
- Assign ARK Number using [Archives West Tools Site](https://archiveswest.orbiscascade.org/tools/) 
- Flag offensive material 
- Complete all required AS fields 
6. Upload record to Archives West using [Archives West Tools Site](https://archiveswest.orbiscascade.org/tools/)
7. Shelve in final location and make note of location in AS

---
### Born-Digital Accessioning and Processing

[section under review]

*The following framework was largely adapted from the [University of Buffalo Libraries Special Collections](https://research.lib.buffalo.edu/digitalpreservation/processing)[^2], Yale Library's [Born Digital Archival Description Guidelines](https://guides.library.yale.edu/c.php?g=934566&p=6736587)[^3], and University of California's [Guidelines for Born-Digital Archival Description](https://github.com/uc-borndigital-ckg/uc-guidelines/tree/master)[^4].*

Like physical collections, born-digital assets transferred or gifted to the department will undergo the same accessioning and processing procedures. For more information on how to accession and process materials, please see the **[Accession]({{ '/content/accessions/rehouse.html' | relative_url }})** and **[Processing]({{ '/content/processing/collection-description.html' | relative_url }})** Manuals. 

Staff members must be certain to include donor documentation and whatever digital storage information there is upon donation. Before beginning the processing stage, staff members will follow a digital processing framework in order to accurately understand what the scope is.

{% capture text %}
1. Reviewing accession record and other documentation about provenance.
2. Identify and document scope and contents of items, and if there are access restrictions (i.e. copyright, personal information, donor restrictions, etc.). 
3. Determine materials that are digital only (hybrid collections) and extent. 
4. Determine collection level information and date range. 
{% endcapture %}
{% include card.html header="Surveying the collection by:" text=text %}

{% capture text %}
1. Determine the priority of processing the collection and the level of access needed. 
2. Identify the scope and level of collection description. 
3. Review descriptive and arrangement needs of collection for patron discovery. Like analog collections, there may be a need for archivists to adjust organization and arrangement.
- No intervention (original order retained)
- Minimal intervention (original order retained; duplicate files donated overtime removed)
- Intervention (original order not retained; re-organized following consultation with donor)
- Post-ingest intervention (ingested into repository in original order; intellectual reorganization taken to all subsequent material to be integrated into single system of arrangement)
{% endcapture %}
{% include card.html header="Formulate a processing plan:" text=text %}

{% capture text %}
1. Review what the media is (i.e. floppy disks, CDs, DVDs, zip drives, electronic transfer, etc.). 
2. Assign a unique identifier (PG, MG, or UG). 
3. Create an inventory for each media storage item using the Media Inventory spreadsheet template. 
4. Add inventory information to ArchivesSpace Resource Record. 
5. Rehouse media if necessary and label with new identifier. 
{% endcapture %}
{% include card.html header="Establish control over removable media storage:" text=text %}

{% capture text %}
1. Capture content off physical storage, perform virus scan, create checksums, and preservation and access copies of assets. 
- See Procedures for Digital Asset Ingesting. 
{% endcapture %}
{% include card.html header="Ingest content:" text=text %}

{% capture text %}
1. Complete the accession and processing procedures in ArchivesSpace using the Spec Practices & Procedures Manual. 
- If using the AS upload template, see the Digital Materials and AS Template guideline. 
- Please note some fields will need alternate wording and/or selections when processing digital assets. For those specific requirements, see the Digital Material Processing and Descriptions in AS guidelines. 
- If Personal Identification Information (PII) is found, discounting accessioning or processing and make a restriction on access note in AS. 
{% endcapture %}
{% include card.html header="Complete procedures in ArchiveSpace:" text=text %}

{% capture text %}
**NOTE:** Some accessions with digital assets have already been ingested via FRED. The full list is located here: Collections with Digital Materials. If a staff member is processing an accession and comes across a type of digital item, check against the list to determine whether ingesting is the next step. If a collection has been fully processed and digital materials had been previously ingested, be sure to change the accession number to the processed collection ID.
{% endcapture %}

{% include alert.html text=text color="info" %}

---
**Footnotes**

[^1]: “The groups of records selected for holdings maintenance projects are chosen after weighing a variety of archival considerations, including intrinsic value, condition, and anticipated use of the records. In some instances it may be appropriate to do no more than rebox, or refolder and rebox a records series; in other cases, it will be appropriate to carry out the complete range of holdings maintenance actions.” (p. 3); “Boxes that are physically damaged (exhibiting such characteristics as broken hinges or missing flaps) and no longer capable of supporting or protecting archival records adequately should be replaced with new storage containers. Boxes of unknown or suspect quality should be tested for pH level and alkaline reserve, to determine whether they should be replaced with new acid-free or low-lignin boxes.” (p. 4); “Folders that are physically damaged and no longer capable of protecting or supporting archival records should be replaced. Folders of unknown or suspect quality should be tested for the pH level and alkaline reserve, to determine whether they should be replaced with new folders.” (p. 4-5). Mary Lynn Ritzenthaler, Preservation of Archival Records: Holdings Maintenance at the National Archives, Technical Information Paper No. 6 (Washington, D.C.: National Archives and Records Administration, 1990).
[^2]: [University at Buffalo, University Libraries. (2023). Digital Records in Special Collections: Processing Born-Digital Records. Retrieved from https://research.lib.buffalo.edu/digitalpreservation/processing](https://research.lib.buffalo.edu/digitalpreservation/processing)
[^3]: [Yale University Library. (2020). Born Digital Archival Description Guidelines. Yale University Library Research Guides. Retrieved from https://guides.library.yale.edu/bddescriptionguidelines](https://guides.library.yale.edu/c.php?g=934566&p=6736587)
[^4]: [University of California Systemwide Libraries. (2017). UC Guidelines for Born-Digital Archival Description. UC Office of the President: University of California Systemwide Libraries. Retrieved from https://escholarship.org/uc/item/9cg222jc.](https://github.com/uc-borndigital-ckg/uc-guidelines/tree/master)