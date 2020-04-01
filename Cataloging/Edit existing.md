# Editing existing MARC records

## 1. In Sierra, search for the collection whose record you want to edit
     
  - Copy the OCLC record number from the **001** field
  - Close the record (you cannot overlay a new record onto an open record)
      
## 2. In Connexion, open the record you want to edit (search: #OCLCnumber)

## 3. Make necessary updates according to the blue/green sheet

   - Note that dates need to be updated in two locations:
      - Fixed fields
      - Collection number
   - Ctrl-D for subfield
      
## 4. Other things to check for:

   - Add ‡e dacs in the **040**, if it isn't there already
   - Remove **545**, update **520**
   - **546 _ _** In English
   - **506 0 _** No restrictions (if there's not already a **506** listing in the restrictions)
   - **856 4 2** the finding aid URL is current
   
## 5. After making the desired edits

  - Click on R
  - Click on the check mark
  - Control headings if needed (Shift + F11)
  - Action > Replace record (Alt + F10)
  
## 6. Bring the record to Sierra

  - Export (F5)
  - Open the record in Sierra
  - Open the summary
    - Update the cat date in the internal note (“lls cat date 16 Feb, 2018”) - "x" for internal note
    - If there are older codes from a previous ILS, they can be deleted (the bottom of the summary should only include the collection call number and the cat date info) 
    - Add "Cataloged FY 2019-20" - "j" for stats field, or macro shortcut if set up (F7 for Jodi) 
    - Save 
    
## 7. Enter in stat sheet under OCLC enhance and Millennium edits sections

## 8. Save to local file (F4)
