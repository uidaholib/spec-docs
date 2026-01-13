---
section: Practices and Procedures
nav_order: 10
title: Digital Collections
---
---

Archival digitization can sometimes turn into a larger project such as creating a digital collection. Departments who usually participate in this initiative include [Special Collections and Archives](https://www.lib.uidaho.edu/special-collections/), [Data and Digital Services](https://www.lib.uidaho.edu/services/dds.html), and the Library's [Center for Digital Inquiry and Learning (CDIL)](https://cdil.lib.uidaho.edu/). A majority of the digital collections are created using [CollectionBuilder](https://collectionbuilder.github.io/). This system generates sites by metadata and powered by static web-technology. 

{% capture text %}
**NOTE:** Metadata used to complete ArchivesSpace Accession and Resource Records for finding aids is *not* the same as metadata for digital collections. Be sure to follow the instructions for creating a digital collection closely.
{% endcapture %}

{% include alert.html text=text color="danger" %}

Before creating a digital collection, consult the Digital Collections Team (DCT). Digital Collection metadata and creation documentation can be found on the University of Idaho Library [Digital Collections Team documentation site](https://uidaholib.github.io/digital-collections-docs/content/dc-team.html).

**Born-Digital Materials**

[This section is out of date and under review]

In some instances, born-digital collections or assets can be made into a digital collection. First ingest files using the [Digital Material Ingest]({{ '/content/processing/digital-ingest.html' | relative_url }}) documentation.

The DROID export metadata sheet may help during the creation of the online collection’s metadata. Creators should compare the information from the DROID sheet to the required fields in the provided csv template. Similar fields that may be useful include the *file name, type, and date*. For example, when creating the digital collection csv metadata sheet for the [Earl Bennet Stock Certificates collection (MG 572)](https://archiveswest.orbiscascade.org/ark:80444/xv839959), the information from the “name” field in the DROIDexport metadata sheet was used as the “filename” in the csv template.

However, this will not always be true and most fields from the DROIDexport may not be used. Staff members still need to look at the digital assets themselves in order to fill out the digital collection spreadsheets properly. For example, the digital assets in MG 572 were inventoried by the donor using Microsoft Excel. This excel document was included as a collection item, and it was used to help fill out the csv template for digital collection creation. The information in the inventory sheet included metadata which was used to fill out the “title” field of the csv template. To fill out the rest of the metadata fields in the csv template, the student worker had to physically look at the digital assets. MG 572 was made up mostly of scans saved as high-resolution jpgs. The scans were of stock certificates and visually included information like the stock company, date, who the stocks were issued to, how many shares, and location information. This provided the student worker with enough context to complete the description, date, and location fields of the csv template. 

After finishing the csv metadata template, copy the appropriate digital files from the Archive Drive onto the **external hard drive used between Spec and CDIL**. This will allow folks to place the images on the web server so they will be viewable in the digital collection. 