---
section: Practices and Procedures
nav_order: 11
title: Digital Collections Procedures for Spec
---


Archival digitization can sometimes turn into a larger project such as creating a digital collection. Departments who usually participate in this initiative include [Special Collections and Archives](https://www.lib.uidaho.edu/special-collections/), [Data and Digital Services](https://www.lib.uidaho.edu/services/dds.html), and the Library's [Center for Digital Inquiry and Learning (CDIL)](https://cdil.lib.uidaho.edu/). A majority of the digital collections are created using [CollectionBuilder](https://collectionbuilder.github.io/). This system generates sites by metadata and powered by static web-technology. 

{% capture text %}
**NOTE:** Metadata used to complete ArchivesSpace Accession and Resource Records for finding aids is *not* the same as metadata for digital collections. Be sure to follow the instructions for creating a digital collection closely.
{% endcapture %}

{% include alert.html text=text color="danger" %}

Before creating a digital collection, consult the Digital Collections Team (DCT). Digital Collection metadata and creation documentation can be found on the University of Idaho Library [Digital Collections Team documentation site](https://uidaholib.github.io/digital-collections-docs/content/dc-team.html).


## Developing a Digital Collection (Spec instructions)

This digital collection creation walkthrough is an adapted version specifically for Spec employees and Spec materials. For fuller documentation, see [Digital Collections at the University of Idaho](https://uidaholib.github.io/digital-collections-docs/) and [CollectionBuilder Docs](https://collectionbuilder.github.io/).

### Scan Materials

- Choose the dpi and file type you should scan to

    {:.table }
    | Type | Scan settings |
    | --- | --- |
    | Photograph, 5x7" or larger | 600 dpi, TIFF, color |
    | Photograph, 5x7" or smaller |	Up to 1200 dpi, TIFF, color |
    | Text | 400 dpi, TIFF, color |
- Name your files appropriately
    - No spaces, no capital letters
    - collectionnumber_boxnumber_foldernumber_itemnumber (ex. mg190_b4_f2-001)
    - Adapt as necessary

### Process Images

- Photograph
    - Create an access copy JPG in Photoshop (File>Automate>Batch...tif>jpg)
    - Straighten, crop, color correct in Photoshop
    - Create low resolution JPG (File>Automate>Batch...access>jpg or 300dpijpg)
- Text document
    - Straighten, crop, color correct in Photoshop
    - Open TIFF in Adobe Acrobat
    - Go to File>Save As Other>Optimized PDF
    - In the Images panel, set Color Images to: 
        - Downsample to 250 ppi
        - Compression JPEG
        - Quality: Medium or High
    - Before batch processing, check your output on a sample document. Zoom to 100% and confirm that the text looks sharp. Check that file size is reasonable (500-1500 KB is reasonable).
    - Send finished PDFs to Andrew for OCR

### Develop Metadata

- Download a blank metadata template: [https://docs.google.com/spreadsheets/d/1dRgG-Xd28gRZ9ErbU6-1YtgNM6gHFEh3IFNOwKzpoRc/copy?usp=sharing](https://docs.google.com/spreadsheets/d/1dRgG-Xd28gRZ9ErbU6-1YtgNM6gHFEh3IFNOwKzpoRc/copy?usp=sharing)
- Decide which fields you need to use, based on these instructions: [https://uidaholib.github.io/digital-collections-docs/content/metadata/02-metadata.html](https://uidaholib.github.io/digital-collections-docs/content/metadata/02-metadata.html). 
    - NOTE: Generally speaking, you can create almost any metadata field you want, based on the nature of the digital collection. However, it may be best to stick with the standard fields if possible.
- Fill in the values, referring to the guidelines at the link above. Of special note for archival collections: 
    - date should be in YYYY-MM-DD, YYYY-MM, or YYYY format. You can estimate to the nearest decade. If you can't estimate, leave this field blank.
    - archival_date is a free text field. This can accommodate ambiguity - undated, decade ranges, month names, etc. If you have a value in the date field, you should also have something in the archival_date field (these can be the same, and they often are the same).
- Do any transcription work for audio/video. 

### Create the Digital Collection

- Create a stub name for the digital collection. It should be short and reflect the name of the digital collection. Create a folder on the objects server with the stub name.
- Process and store files
    - Gather objects in a single folder
    - Generate object derivatives (see [https://collectionbuilder.github.io/cb-docs/docs/objects/derivatives/](https://collectionbuilder.github.io/cb-docs/docs/objects/derivatives/))
    - Copy objects and derivatives to their proper folders on the objects server
    - Copy objects, derivatives, and preservation scans to the archive drive, accompanied by a README explaining the who/what/when/where/why of the folder
- Check that metadata is complete
- On GitHub, choose the digital collection template that best fits your digital collection; 
    - base-digital-collections-template: standard, good for big photograph collections or a mixture of photos and text
    - documents-digital-collections-template: for collections that are primarily text documents
    - campus-collections-template: for collections of university materials
    - ijc-collection-template: for collections created from IJC materials
    - oral-history-collections-template: for oral history collections
- Start a new collection branch in GitHub within your chosen template, using your new stub name
- Configure your collection in VSC
    - Add metadata spreadsheet to _data
        - NOTE: DO NOT open spreadsheet in Excel. Download as .csv directly from Google Sheets and drag directly into VSC.
    - Edit _config
        - Do not change url, source-code, or digital-assets
        - Update baseurl with /digital/stubname
        - Create title, tagline, description, keywords
        - Update metadata with stub name
    - _data/theme.yml
        - Add featured image object id
        - Configure browse, subjects, locations, map, etc., as needed
    - Page configs
        - Other _data configs
- Write interpretive content (About page)
    - First paragraph should include information about the digital collection
    - Use short paragraphs and lots of headings
    - Start with h2 level (##) and go only one step up or down in successive headings. 
    - Leave blank lines between each heading and paragraph.
    - Use meaningful text in hyperlinks. Use simplified hyperlinks if linking to items within the same collection
    - Don't use double spaces after periods
    - Follow citation format. Preserve citation links with Perma.cc
- Preview and review collection
    - Check Review page items
- Send out for Quality Control

### Launch Checklist
- Promo blurbs:
    - BN
    - Library updates page
    - Library newsletter
    - Daily Register
- Mention at weekly update
- Library TV screen
- Harvester post
- Fill out the tracking sheet

### Final Steps
- Update the archival finding aid to include link(s) to the digital collection
- Upload digital collections files to the archive drive and include a README (contact digital archivist)