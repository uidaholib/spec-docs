---
section: Processing Manual
nav_order: 6
title: Errors in ArchivesSpace
---

Sometimes when loading xml files into ArchivesSpace (AS), there will be errors. These occur because of outdated formats used to create older finding aids. When an error occurs, AS does give hints as to why it's having issues. *These aren't always readable or understandable*, but below is an example of how and where to look to try and troubleshoot.

{% capture text %}
**NOTE:** If troubleshooting doesn't work or is too time consuming, contact Orbis Cascade with the issue using the [Help Request Form](https://www.orbiscascade.org/programs/osdc/help-request/)
{% endcapture %}

{% include alert.html text=text color="danger" %}

## ArchiveSpace Error Example
###### *See [Importing Archives West files to ArchivesSpace](https://vandalsuidaho.sharepoint.com/:w:/r/sites/Storage-Library/Documents/spec/Departmental%20Projects/Collections%20To%20Add%20to%20ArchivesSpace/Importing%20Archives%20West%20files%20to%20ArchivesSpace.docx?d=w0d82bda19aab4af7a6652f358e8dc60c&csf=1&web=1&e=SKCUJC) for full importing instructions.*
---
Scenario: Importing the [Agricultural Engineering Department Records](https://archiveswest.orbiscascade.org/ark:80444/xv02059)'s xml into ArchivesSpace, but it fails and an error occurs.
{% include figure.html img="aspace-error.png" alt="" caption="" width="" %}

Notice in the error box, it will say what error is found.
{% include figure.html img="aspace-property-missing.png" alt="" caption="" width="" %}

"Missing required property" means this is a **level** issue aka: series, sub-series, file, item, etc.
<p>The error box also shows where in the xml file the error is occurring.</p>
{% include figure.html img="error-find.png" alt="" caption="" width="" %}

In the box, scroll to the right to read the string of code under "For JSONModel" section. Usually, you can see **where** in the xml file the error is occurring because it will say "title".
{% include figure.html img="error-title.png" alt="" caption="" width="" %}

Next, open the xml file in Visual Studio Code, and find the title in the code.
{% include figure.html img="find-in-xml.png" alt="" caption="" width="" %}

Notice in the original Archives West finding aid, this section should be a series but it doesn't have a level associated with it. This is why there is an error.
{% include figure.html img="missing-property-level.png" alt="" caption="" width="" %}

Add the level information and save the xml file.
{% include figure.html img="add-level.png" alt="" caption="" width="" %}

Now the xml file will import into ArchivesSpace without errors!
{% include figure.html img="done.png" alt="" caption="" width="" %}

