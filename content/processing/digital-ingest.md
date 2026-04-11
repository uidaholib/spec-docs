---
section: Processing Manual
nav_order: 12
title: Digital Processing Walkthrough
---

*Last updated 03-24-2026*

## When to Ingest

Born-digital materials are usually ingested off of the original storage media during the processing stage (from original storage media or online transfer) or during processing (from original storage media). Reasons to ingest at the accession stage:
- Donor is donating digital copies rather than originals
- Storage media is fragile or deteriorating
- Donation is an online transfer (via email attachment, cloud transfer, etc.)

Regardless of when digital materials are ingested, they should be transferred to the Spec partition of the archive drive.

NOTE: If the media seems at risk for viruses or other harmful material (unknown provenance, poor tech practices by donor, etc.), either:
- Avoid the media by refusing donation or deaccessioning
- Quarantine for 30 days (to allow virus scanning software to update fully) and open in a non-networked workstation

For more acquisition information, see [Acquisition Practices](https://uidaholib.github.io/spec-docs/content/introduction/acquistion.html).

## Processing Procedures: Physical Storage Media

Processing Procedures: Physical storage media

Step 1: Prep
- Identify the storage media type (ZIP drive, USB drive, floppy disk, hard drive, CD, DVD, etc.).
- Retrieve the "Digital Archives Ingest" (DAI) external hard drive.
- Plug both the DAI and the storage media into your workstation (see [] for a list of Spec equipment).

Step 2: Virus check
- Right click on the storage media and Scan with Sophos Endpoint
- If the virus check detects threats, do not open the media. Your options:
    - Contact the donor
    - Deaccession the material

Step 3: Create folders
- On the DAI drive, in either the Accession folder or the Processed folder, create a new folder with the accession or processed collection number and name (e.g., PG 104 (Avista Aerial Photographs of Latah County).
- On the DAI drive, open README_TEMPLATE in a text editor and save a copy to the accession or processed collection folder you just created, renaming it README_[collection number] (e.g., README_pg104). 
- Fill in the top fields of the README with information about the media you are processing, and continue updating the README as you process the media. 
- Within the new accession/collection folder, create two more folders: Metadata and Objects.

Step 4: Transfer objects to DAI drive
- For a basic transfer, use Bagger.
    - Click Create New Bag. Make sure <no profile> is selected. Click OK.
    - Click File>Add Data. Find the original storage media and select all files and folders. Click OPEN.
    - Click Save Bag As... on the right side of the menu bar.
        - Locate your Objects folder on the DAI drive. Filename should be the accession/processed collection number plus the media item number and _bag (ex. pg104_disc001_bag). 
        - Serialize Type = none
        - Generate Tag Manifest = checked
        - Tag Manifest Algorithm = md5
        - Generate Payload Manifest = checked
        - Payload Manifest Algorithm = md5
    - When bag saves successfully, click OK.
- For disk imaging, use AccessData FTK Imager.
    - Floppy disks, ZIP/USB drives, hard drives: 
        - File > Create disk image
        - Source > Logical Drive > NEXT
        - Select drive or browse to find media. FINISH. 
        - Create Image, select: Verify images after they are created and Create directory listing of all files in the image. Add.
        - Select Image Type, select: RAW. NEXT.
        - Evidence Item Info, select: 
            - Case No. = Accession/Collection ID
            - Evidence No. = Media ID (e.g., disc011)
            - Unique Description = blank
            - Examiner = your name
            - Notes = blank
            - NEXT
        - Select Image Destination > Browse > navigate to Objects folder on the DAI drive
        - Image Filename, enter: 
            - Identifier (e.g., pg104_disc001)
            - Select 0 for Image Fragment Size and Image - Compression Size
            - FINISH
    - CDs, DVDs:
        - File>Create disk image
        - Source>Logical Drive>NEXT
        - Select drive or browse to find media. FINISH.
        - Create Image, select: Verify images after they are created and Create directory listing of all files in the image. Add.
        - Select Image Destination>Browse>navigate to Objects folder on the DAI drive.
        - Image Filename, enter: 
            - Identifier (e.g., pg104_disc001)
            - Select 0 for Image Fragment Size and Image - Compression Size
            - FINISH

Step 5: Generate metadata and checksums with DROID
- File>Save As>navigate to Metadata folder
    - Enter accession/processed collection ID as filename. Save.
- Select ADD button (green plus sign). Navigate to Objects folder > data folder. OK.
- Be sure that checksum is being generated. Tools > Preferences > Check "generate hash for each file." Select MD5.
- START
- Once finished, select EXPORT.
    - Select profile.
    - Select Export Profiles. Save file as .csv in Metadata folder. Filename should be accession/collection ID + _DROIDexport (e.g., pg104_DROIDexport).
- Delete DROID profile from Metadata folder (a .pdf)
- Open .csv to check that hash (checksums) and MIMTYPE were reported
- Do not save profile when closing DROID

Step 6: Move to archive drive
- Full update README.
- Transfer package of files to either the Accessions or Processed Collections folder of the Spec partition of the archive drive.
- Label media and place back in collection.

Step 7: Description and resource record
- Fill in an inventory spreadsheet and resource record as usual, noting extent in bytes when appropriate. 
- Note archive drive location in "Existence and Location of Originals" or "Existence and Location of Copies."


Processing Procedures: Online transfer

Step 1: Prep
- Retrieve the "Digital Archives Ingest" (DAI) external hard drive and plug into your workstation.
- Create a staging folder on the DAI drive.
- Download the donated/transferred material to the DAI drive staging folder.

Step 2: Virus check
- Right click on the donated/transferred material and Scan with Sophos Endpoint
- If the virus check detects threats, do not open the media. Your options:
    - Contact the donor
    - Deaccession the material

Step 3: Create folders
- On the DAI drive, in either the Accession folder or the Processed folder, create a new folder with the accession or processed collection number and name (e.g., PG 104 (Avista Aerial Photographs of Latah County).
- On the DAI drive, open README_TEMPLATE in a text editor and save a copy to the accession or processed collection folder you just created, renaming it README_[collection number] (e.g., README_pg104). 
- Fill in the top fields of the README with information about the media you are processing, and continue updating the README as you process the media. 
- In README, note sender, date of transfer, method of transfer. 
- Within the new accession/collection folder, create two more folders: Metadata and Objects.

Step 4: Transfer objects
- Use Bagger to move the donated/transferred materials from their staging folder to the Objects folder.
    - Click Create New Bag. Make sure <no profile> is selected. Click OK.
    - Click File>Add Data. Find the staging folder and select all files and folders. Click OPEN.
    - Click Save Bag As... on the right side of the menu bar.
        - Locate your Objects folder on the DAI drive. Filename should be the accession/processed collection number plus the media item number and _bag (ex. pg104_transfer001_bag). 
        - Serialize Type = none
        - Generate Tag Manifest = checked
        - Tag Manifest Algorithm = md5
        - Generate Payload Manifest = checked
        - Payload Manifest Algorithm = md5
    - When bag saves successfully, click OK.

Step 5: Generate metadata and checksums with DROID
- File>Save As>navigate to Metadata folder
    - Enter accession/processed collection ID as filename. Save.
- Select ADD button (green plus sign). Navigate to Objects folder > data folder. OK.
- Be sure that checksum is being generated. Tools > Preferences > Check "generate hash for each file." Select MD5.
- START
- Once finished, select EXPORT.
    - Select profile.
    - Select Export Profiles. Save file as .csv in Metadata folder. Filename should be accession/collection ID + _DROIDexport (e.g., pg104_DROIDexport).
- Delete DROID profile from Metadata folder (a .pdf)
- Open .csv to check that hash (checksums) and MIMTYPE were reported
- Do not save profile when closing DROID

Step 6: Move to archive drive
- Full update README.
- Transfer package of files to either the Accessions or Processed Collections folder of the Spec partition of the archive drive.
- Delete the staging folder from the DAI drive.
- Retain any emails or other messages from donor as part of the accession record, either in SharePoint or in the accessions binder.

Step 7: Description and resource record
- Fill in an inventory spreadsheet and resource record as usual, noting extent in bytes when appropriate. 
- Note archive drive location in "Existence and Location of Originals" or "Existence and Location of Copies."
