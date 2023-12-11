---
section: Practices and Procedures
nav_order: 2
title: Ingesting Digital Materials
---
If an archivist comes across digital storage media within a collection or in a donation/transfer, materials are usually ingested during the processing stage. There is software and procedures one should be familiar with in order to ingest properly. Materials ingested are then saved on the Archive Drive.

<div class="text-center mb-2">
    <a href="#{{ 'Software and Programs Used' | slugify }}" class="btn btn-secondary my-2 mx-1">Software and Programs</a>
    <a href="#{{ 'Procedures' | slugify }}" class="btn btn-secondary my-2 mx-1">Procedures</a>
</div>

---
## Software and Programs

These programs are installed on the FRED computer (located in the main office space).

{:.table .table-bordered}
| Program/Software | Description |
| - | ----- | 
| Sophos Endpoint | Scans storage media for threats or viruses|
| Notepad, Notepad++ | Keeps storage media record of information in a plain text document. |
| DROID (Digital Record Object Identification) | Developed by the National Archives to profile wide range of file formats. Creates inventory list with checksums, modification date, file format information, etc. |
| Bagger | Developed by the Library of Congress to bag files into a BagIt file structure (set of hierarchical file layout conventions for storage and transfer of arbitrary digital content). Suitable for reliable storage and transfer. |
| AccessData FTK Imager | Previews recoverable data from a disk of any kind. |
| Java | Programming language and computing platform. Needed for DROID and bagger programs. |

---
## Procedures

*Follow these steps to ingest the digital materials into the Archive Drive.*

#### STEP 1: 
Identify the type of storage media which contains the materials (i.e. zip/usb drive, SD card, floppy disk, hard drive, CD, DVD, etc.). Then retrieve the “Digital Archives Ingest” (DAI) external hard drive. (Currently located at the FRED station.) 

#### STEP 2:
Plug in DAI drive & whatever the media storage. In File Explorer, find the storage media drive. Right click on the media and select Scan with Sophos Endpoint. Notice whether any threats/viruses were detected. 

#### STEP 3: Creating a folder. 
- Go to DAI drive > Accession OR Processed folder. Then create a new folder with the accession OR collection ID the digital assets belong to. 
    - Ex: MG 333 (Moscow Meals on Wheels records) 
    - Ex: UA 1987-25 (Jane Vandal papers) 
- In the new folder, create 2 sub-folders labeled “Metadata” & “Objects”. These will house the metadata & files after transfer.

#### STEP 4: Creating & updating a log in Notepad++. 
- Go to DAI, right click on “README_TEMPLATE”, select Edit with Notepad++. 
- Save the file as “README_Accession/CollectionID_CollectionTitle” in the “Metadata” folder previously created. 
    - Ex: README_UG068_AthenaRecords 
- Update the file with the collection information. See the following bullets for examples. 
    - *Accession/Collection ID:* UG 068 
    - *Collection Title:* Athena records 
    - *Digital Objects in Original:* # of digital objects being ingested 
    - Media information 
        - mg068_disc001 
        - Title on media (whatever is written on media) 
        - Data on media (date written on media)
            - Can determine date by viewing files. 
        - Description (anything else written on media/discovered) 
    - *Virus Scan:* Note whether a virus scan resulted in issues. Otherwise, type “Completed virus scan on all disc images & file directories. No viruses found.” 
    - If transferring more than one storage item, after “Media Information” add another section of media information. Continue pattern until all media is accounted for. 
    - SAVE this file.

#### STEP 5: Creating disc images. 
##### For floppy disks, zip/usb drives, and hard drives: 
- Open AccessData FTK Imager from desktop.  
- Select *File* then “Create disk image” 
- Select *Source*
    - Choose “Logical Drive” and click *NEXT*. 
- Select the drive or browse to find 
    - For usb, zip, floppy: may say USB (FAT) 
    - Be sure to select correct media drive and select *FINISH*. 
- In “Create Image” box, select: 
    - *Verify images after they are created* 
    - *Create directory listing of all files in the image*
    - Select “Add” 
- In “Select Image Type” box, select *RAW* & click NEXT. 
- In “Evidence Item Info” box: 
    - Case No. = Accession/Collection ID 
    - Evidence No. = Media ID (ex: disc001, cd005, etc.) 
    - Unique Description = blank 
    - Examiner = person working on ingest 
    - Notes = blank 
    - Click NEXT 
- In “Select Image Destination” box: 
    - Click Browse and navigate to DAI drive > Accession OR Processed folder > Accession OR Collection folder > Object folder. 
- In “Image Filename” field enter identifier for media 
    - Ex: MA2007_18_disc005 
    - Select *0* for “Image Fragment Size” & “Image Compression Size” 
    - Click FINISH 
- In “Create Image” box select START. (Note this might take some time.) 
- When completed, go to File Explorer 
    - Move disk image reports (excel and text documents) to DAI > Accession OR Processed Collections > appropriate folder > Metadata folder. 

##### For optical drives (CDs/DVDs): 
- Open AccessData FTK Imager from desktop.  
- Select *File* then “Create disk image” 
- Select *Source*
    - Choose “Logical Drive” and click NEXT. 
- Select the drive or browse to find 
    - Be sure to select correct media drive 
- Select *FINISH*. 
- In “Create Image” box, select: 
    - *Verify images after they are created*
    - *Create directory listing of all files in the image*
    - Select “Add” 
- In “Select Image Destination” box: 
    - Click *Browse* and navigate to DAI drive > Accession OR Processed folder > Accession OR Collection folder > Object folder. 
    - In “Image Filename” field enter identifier for media
        - Ex: MA2007_18_disc005     
    - Click FINISH 
- In “Create Image” box select START. (Note this might take some time.) 

**When completed, go to File Explorer**
- Move disk image reports (excel and text documents) to DAI > Accession OR Processed Collections > appropriate folder > Metadata folder.

#### STEP 6: Transfer files. 
- Open Bagger program on desktop.
{% capture text %}
**NOTE:** May not open. If error occurs, in File Explorer open Documents. Double click on “JavaInstall.” Once install finishes, try Bagger again.
{% endcapture %}
{% include alert.html text=text color="danger" %}
- Click “Create New Bag” 
    - Make sure *< no profiles >* is selected. Click “OK.” 
- Then go to File > Add Data 
    - Find the storage media using the drop-down menu 
        - Select all the files and folders 
        - Click OPEN. 
- Click “Save Bag As...” (from menu banner)
    - Browse to find the Digital Archives Ingest (DAI) drive 
        - Then find the appropriate accession or processed collection folder and save in the “Objects” folder. 
            - File name should be the accession/processed collection ID_disc#_bag 
                - Ex: MA2023-25_disc001_bag 
- Make sure the following are selected. 
    - Serialize Type = None
    - Generate Tag Manifest = checked 
    - Tag Manifest Algorithm = md5 
    - Generate Payload Manifest = checked 
    - Payload Manifest Algorithm = md5 
    - When bag saves successfully, click “OK.” 

#### STEP 7: Generate metadata. 
- Open *DROID* software on desktop
- Select File then “Save As” and navigate to DAI > Accessions OR Processed Collections > appropriate folder > Metadata folder 
    - Enter the accession/collection ID as the file name 
    - Ex: UG068_disc001 
    - Select “Save” 
- Select the ADD button (green plus sign) 
- Go to DAI > Accessions OR Processed Collections > collection folder > Objects > data folder. 
    - Select the files/folders to be analyzed 
    - Click “OK” 
- Be sure that *checksum* is being generated. 
    - Tools > Preferences > Check “generate hash for each file” 
    - Select MD5 
- Click START 
- Once finished, select EXPORT 
    - Select box for *profile*
    - Select “Export Profiles” 
        - Save file as CSV in DAI > Accessions OR Processed Collections > collection folder > Metadata folder 
        - File name should be accession/collection ID + “DROIDexport”
            - Ex: UG068_disc005_DROIDexport.csv 
- Delete DROID profile from Metadata folder (the pdf file) 
- Open CSV file when finished to check that hash (checksums) and MIMTYPE were reported 
- **DO NOT save profile when closing DROID program**

#### STEP 8:
Label media with Accession OR Collection ID. If from a physical collection, place back in container pulled from.  