---
section: Processing Manual
nav_order: 7
title: Archives West Finding Aid
---
---

After a Resource Record in completed in ArchivesSpace, the next step is to upload the information into Archives West.

In ArchivesSpace, find the Resource Record that is ready to be uploaded. Once found:

#### Step 1:

- To the right of the record, click on the **Export** button.
- Then *hover* over the **Download EAD**. A small window will pop up.
    - Make sure the top **4** boxes are checked (do not check "EAD3 schema"). 
- Then click on **Download EAD**.

{% include figure.html img="ead.jpg" alt="downloading ead" caption="" width="" %}

- An .xml file will download.

---
#### Step 2:

- Open and log into the [Archives West Management Tools](https://archiveswest.orbiscascade.org/tools/login.php?redirect=/tools/) site.
    - Username and password information can be found in the Spec Accounts document on SharePoint.
- Under the *Document Submission* section, click **ArchivesSpace EAD Converter**. 

{% include figure.html img="ead-converter.jpg" alt="converting ead file" caption="" width="70%" %}

- Choose the .xml file you downloaded from ArchivesSpace, and click **Convert EAD**.
- Click **Download File**.
    - The new downloaded file's name should begin with NTD and the collection number.
        - Example: NTDMG009.xml
- Go back to the Tools homepage.

{% include figure.html img="convert.jpg" alt="converting ead file" caption="" width="80%" %}

---
#### Step 3:

- Under the *Document Submission* section, click **Document Validation**.
- Choose and upload the NTD downloaded file and click **Validate File**. 
    - A green message should pop up saying the file is valid.
    - If there is an issue in the record, there will be an error message in red.
        - Check Resource Record for potential error. Consult colleagues if unable to determine the issue.
- Go back to the Tools homepage.

{% include figure.html img="document-val.jpg" alt="validating ead" caption="" width="80%" %}

---
#### Step 4:

- Under the *Document Submission* section, click **Compliance Checker**.
- Choose and upload the NTD downloaded file, check *Required/Mandatory BPG Only*, and click **Check Compliance**.
    - If an error occurs, the text will be in red.
    - If the beginning section contains an error, the file will not be loaded the Archives West.
        - Check Resource Record for potential error. Consult colleagues if unable to determine the issue.
    - If the following sections contain errors, check the Resource Record.
        - These errors can get pushed through and the finding aid will load on Archives West. Consult colleagues if unable to determine if an issue should be/can be resolved.
- Go back to the Tools homepage.

{% include figure.html img="compliance.jpg" alt="checking compliance" caption="" width="80%" %}
{% include figure.html img="compliance-issue.jpg" alt="checking compliance issues" caption="" width="80%" %}

---
#### Step 5:

- Under the *Document Submission* section, click **Document Preview**.
- Choose and upload the NTD downloaded file and click **Preview Finding Aid**.
- A window will pop up with a preview of what the finding aid will look like on Archives West. 
    - Check for any issues. Small changes - like spelling errors- can be made in the .xml file by opening it in Visual Studio Code (VSC) (a program which should be installed on computer).
        - Save changes, the upload the file to preview it again.
- Go back to the Tools homepage.

{% include figure.html img="preview.jpg" alt="finding aid preview" caption="" width="80%" %}

---
#### Step 6: 

- Under the *Document Submission* section, click **Document Submission**.
- Choose the correct ARK associated with the Resource Record. Click **Use ARK**.
- In the next window, choose and upload the NTD downloaded file and click **Preview Finding Aid** (to double check final touches).
- Click **Upload File**. This may take some time.
    - If there are errors, the text will be in red.
    - Refresh the page to view the link to the newly created finding aid.
- Process complete.
