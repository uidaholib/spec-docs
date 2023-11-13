---
section: Processing Manual
nav_order: 8
title: Resource Record - Extents
topics: 
---

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