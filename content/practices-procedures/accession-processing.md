---
section_id: Practices and Procedures
nav_order: 2
title: Accession and Processing Procedures
---
<div class="text-center mb-2">
    <a href="#{{ 'Accession Procedures' | slugify }}" class="btn btn-secondary my-2 mx-1">Accession Procedures</a>
    <a href="#{{ 'Processing Procedures' | slugify }}" class="btn btn-secondary my-2 mx-1">Processing Procedures</a>
    <a href="#{{ 'Born-Digital Accessioning and Processing' | slugify }}" class="btn btn-secondary my-2 mx-1">Born-Digital Accessioning and Processing</a>
</div>
---

*Last updated 03-24-2026*

## Accession Procedures

If materials are deemed appropriate for inclusion in Spec, they will be accessioned. Manuscript, university, or photograph collections that have been accessioned will be noted with an identifying number beginning with MA or UA. For a step-by-step guide to accessioning, see the [Accession Manual]({{ '/content/accessions/rehouse.html' | relative_url }}).

---
## Processing Procedures

Accessioned materials are made more useful and accessible through processing. Even a minimal level of processing should be the goal for all collections. While some collections may warrant a very thorough processing, box or folder-level descriptions should suffice in most instances. The level of detail should be determined by the complexity or variety of materials, the size of the collection, and a professional assessment of the collection's importance. This is a subjective process. For a step-by-step guide, see [Processing Manual]({{ '/content/processing/collection-description.html' | relative_url }}).

---
## Born-Digital Accessioning and Processing

Accession and resource records for born-digital materials transferred or gifted to the department will have much of the same information as accession and resource records for analog materials. Please see the Accession and Processing Manuals for information on filling out accession and resource records in ArchivesSpace. 

While the information recorded in both analog and born-digital accession and resource records is mostly the same, accessioning and processing practices may differ significantly. For a step-by-step guide, see [digital section of Accession Manual under construction] and [digital section of Processing Manual under construction]

### Background

The department's digital ingest and processing practices are currently evolving (as of February 2026). 

Between late 2018 and late 2023/early 2024, Special Collections and Archives used a workstation with a Forensic Recovery of Evidence Device (FRED); this workstation included tools/capabilities such as a Tableau write-blocker, Sophos Endpoint for virus detection, bulk_extractor (used in part for PII detection), DROID for metadata, Bagger for moving materials, FTK Imager for disk imaging, and possibly some others. You may see evidence of such tools in older accession and resource records and in files on the archive drive. 

Around late 2023/early 2024, OIT may have imaged the FRED and then attempted to update it to Windows 11. Afterward, the FRED no longer worked properly. 

Since then, Spec employees have attempted to reconstruct an digital archival processing workflow that meets professional standards, a process hampered by employee turnover and loss of workplace knowledge. The current effort is shaped by a few key ideas:
- Software and hardware should be modular and easily replaced, so as to avoid losing all processing capacity due to the failure of one piece of equipment
- Open-source, well-documented, and frequently-updated software tools are prioritized
- Documentation of local practices is thorough and regularly updated

As of February 2026, the digital archival processing workflow includes important steps such as bagging materials with Bagger, documenting metadata and creating checksums with DROID, disk imaging with FTK Imager, and scanning for viruses with Sophos Endpoint. Important elements that are still missing include PII checking, the inclusion of a write blocker, and a standard process for archive drive deposits. Resolving these steps will include further coordination with other Library employees using the archive drive, purchasing a Tableau write blocker, and the digital archivist learning to use BitCurator. 

For a list of Spec's digitization equipment, see [Spec Equipment]({{ '/content/tips-tricks/scanners.html' | relative_url }})


