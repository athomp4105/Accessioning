# Creating new MARC records

## Create a new record

1. Select collection for which you will create a record
   - File > Local File Manager > xx.bib.db
   - Double click, close
2. New mixed material catalog record: Ctrl-Shift-I
3. Bring up constant data (template): Ctrl-B
   
   OR
   
4. Identify record to use to derive new record
   - F3 brings up save file
   - Choose record, copy OCLC number
   - Paste OCLC number into search box
5. Edit > Deruve > New master record (Ctrl-Alt-C)
   - Yes to transfer fixed field values
   
## Completing the fields

If using constant data, most of the fixed fields should be set and the fields that need completing should be clear (Ctrl-Shift-I, Ctrl-B, enter name of constant data template) 

Fixed fields mostly remain the same

### Fixed Fields

**Date(s)**

Select type of date (i: inclusive; s: single); enter dates 

**Country/location)**
  
 Enter country/location (xxu: US; ncu: NC)
 
 ### 040
 
 enter ‡b eng and ‡e dacs **(Ctrl-D to insert ‡)**

If materials in a language other than English are present:

  - 041 _ _ ‡a lang code, repeat ‡a as needed
  
### 100 : Creator

Copy and paste from finding aid
 
  - Right click > Control single heading (F11)
  - ‡d for dates, ‡c for qualifier
  - Person: 100 1 _; Family 100 3 _
  - See Michelle's documentation for forming family and other headings
  
### 245 1 0 : Title

Copy and paste from finding aid

  - If no creator, 245 0 0 (no other changes)
  - Collection in lowercase
  - ‡f for dates, ‡g for bulk dates
  - NO period at end of dates
  
### 300 _ _ : Extent

**"approximately XXX ‡f items ‡a (xx ‡f linear feet)** (no period at end)

  - Remove, edit as needed depending on collection

### 500 _ _ : Citation note

**"In the xxx, University of North Carolina at Chapel Hill (#)"**

  - Possibly other notes, depending
  
### 520 8 _ : Abstract scope and content

Copy and paste abstract scope and content from finding aid (no period at end)

### 506 1 _ : Access restrict

  - Flashers have a more detailed note here, but no other special treatment (no period at end)
  - If no restriction, use **506 0 _ No restrictions**
  
### 530 _ _ : Additional form of material

No period at end

### 540 _ _ : Use restrict

No period at end

### 541 _ _ : Source of Acquisition

**"Acquired ‡d date"** (no period at end)

### 544 1 _ : Related materials

**"See also ‡d collection name (#) in the ‡a collection, University of North Carolina at Chapel Hill"**

### 546 _ _ : Language note

**"In English"** (no period at end)

### 600/610/650/651 : Subject access fields

  - Copy and paste subject headings from finding aid
  - Subfield codes
    - ‡d dates
    - ‡v form
    - ‡x general
    - ‡y chronological
    - ‡z geographic
  - Clean up mess
  - Control headings 
    - Shift + F11 for all
    
### 856 4 2 : Electronic Location and Access  

**"‡3 Finding aid ‡u URL"**

## Finishing up

1. Click on the R in the menu bar

2. Click on the green check next to the R

   - Make any corrections as instructed, if needed
   
3. Click on the yellow up arrow button, two down from R

   - This creates the OCLC#, note it on the blue sheet

4. Run marcro: Ctrl-J
 
   - this adds 099, 049, 949
   - For a new collection:
     - Choose title not in Millennium
     - Copy and notes
     - Have 099 local call #
     - ‡a collection # (include leading zero for SHC collection)
   - For a collection with a collection-level record in Sierra:
     - Choose title in Millennium
     - Copy and notes
     - Have 099 local call #
     - ‡a collection # (including leading zero for SHC collection)
     
5. Bring to Sierra

   - Export using green arrow button (F5)
   - Open Sierra, search by title or local call number
   - Hit summary, confirm item record is there
   - Add STATS note- "Cataloged FY 2019-20" using "j" or macro if set up (e.g. F7)
   - For a collection with a collection-level record in Sierra, edit status in item record and edit initials and cat date
   - Save
   - Close pop up window in Connexion
   
6. Enter in stat sheet

7. Hit F4 to save to local save file

8. Enter OCLC # in Proc Rec

   - TS > archival > processing database > processing_database.db


