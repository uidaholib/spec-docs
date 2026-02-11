---
section: Processing Manual
nav_order: 8
title: Labeling and Shelving
---
<div class="text-center mb-2">
    <a href="#{{ 'Labeling Boxes' | slugify }}" class="btn btn-secondary my-2 mx-1">Labeling Boxes</a>
    <a href="#{{ 'Shelving Materials and Linking Locations' | slugify }}" class="btn btn-secondary my-2 mx-1">Shelving and Linking Locations</a>
    <a href="#{{ 'Creating or Editing Location Records in ArchivesSpace' | slugify }}" class="btn btn-secondary my-2 mx-1">Creating or Editing Location Records</a>  
</div>

### Labeling Boxes

Fill out the [Box Template](https://vandalsuidaho.sharepoint.com/:w:/r/sites/Storage-Library/Documents/spec/Collections/Accessions/Box_Label_template.docx?d=we3ba908310825c1ea33bb3e6196f877f&csf=1&web=1&e=rM2Mxc) with the collection ID, title, date range, and the box number. For collections that have more than one box, make sure to put “Box 1 of” and then whatever the final box total is. 

{% capture text %}
**NOTE:** Try not to adjust the label sizes in the Word doc.
{% endcapture %}

{% include alert.html text=text color="warning" %}

Before printing, be sure to find the label paper (next to the small grey HP printer). Place a piece in the paper feeder, not a tray. After that, feel free to print. Place the labels on the appropriate box.

---
### Shelving Materials and Linking Locations

Consult with colleagues, if needed, about where an appropriate place is to house the collection. Make note of the row, section, and shelf each box is on.  

Return to *Resource Record* in ArchivesSpace and scroll to the **Instances** field. It should look like this:

{% include figure.html img="instances.jpg" alt="instances field" caption="" width="50%" %}

To link location information: 
1. Click on the blue Top Container button, and then click **View.** 
2. A window will pop up with the container details. Click **Edit.** 
3. In the Locations field, click **Add Location** (to the right). 

{% include figure.html img="locations.jpg" alt="locations field" caption="" width="80%" %}

All cage locations should be in ArchivesSpace. From the dropdown menu, select “Browse.” A window with then come up and look like this: 

{% include figure.html img="browse-location.jpg" alt="locations field" caption="" width="80%" %}

When searching for a location, filtering the result by Room is beneficial. After filtering to the area, you’re searching for, in the text box type in the row information.  
- For example, if you’re putting a collection in Cage 1, in Row 113, select “Cage 1” from the Room. Then type in “113.” 
- Once you find the location you need using the row, section, and shelf information you gathered, select the correct result. Then click **Link to Locations.** After linking, your screen will return here with the newly added location information.

Be sure to click **Save Top Container.** Now when you go back to the Resource Record and scroll to the Instances, the boxes will have locations attached to them.

{% capture text %}
**WARNING:** When editing a box's location, make sure you aren't editing the actual *location* information as shown below. Changing this information doesn't change box information, it changes the entire location record.
{% endcapture %}

{% include alert.html text=text color="danger" %}

{% include figure.html img="location-in-as.jpg" alt="locations record" caption="" width="80%" %}

---
### Creating or Editing Location Records in ArchivesSpace

If shelving a collection and there is no location record in ArchivesSpace, **create one**.

{% capture text %}
**NOTE:** Always double check if there is a location record to eliminate duplicate work!
{% endcapture %}
{% include alert.html text=text color="info" %}

- In ArchivesSpace, click **Create**.
- From the drop-down menu, hover over **Location**.
- Choose either *Single Location* or *Create Batch Locations*
    - usually select *Single Location*

{% include figure.html img="create-loc.jpg" alt="creating locations" caption="" width="50%" %}

- Fill in New Location fields: 

{:.table .table-bordered}
| Field | Required | Content | Examples |
| - | ----- | -------- | -------- |
| Temporary? | No | Skip |
| Building | Yes | Type in: **UI Library** |
| Floor | Yes | Type in: **Basement** |
| Room | Yes | Type in storage area location. | Bunker, Cage 1, Cage 2, etc. |
| Area | No | Skip |
| Barcode | No | Skip |
| Classification | No | Skip |
| Coordinate Label 1 | Yes | Type in: **Row** |
| Coordinate Indicator 1 | Yes | Numerical | 1, 2, 3, etc. |
| Coordinate Label 2 | Yes | Type in: **Section** |
| Coordinate Indicator 2 | Yes | Numerical | 1, 2, 3, etc. |
| Coordinate Label 3 | Yes | Type in: **Shelf** |
| Coordinate Indicator 3 | Yes | Numerical | 1, 2, 3, etc. |
| Location Profile | No | Skip |
| Repository | No | Skip |

- When finished filling out fields, click the blue **Save Location** button.

- To simply *edit* a location record, browse for the location and once found click the blue **Edit** button. Then edit necessary fields.

{% include figure.html img="edit-loc.jpg" alt="editing locations" caption="" width="100%" %}