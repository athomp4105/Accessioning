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

- If using constant data, most of the fixed fields should be set and the fields that need completing should be clear (Ctrl-Shift-I, Ctrl-B, enter name of constant data template) 

- Fixed fields mostly remain the same

  - Select type of date (i: inclusive; s: single); enter dates 
  - Enter country/location (xxu: US; ncu: NC)
  
- **040:** enter ‡b eng and ‡e dacs **(Ctrl-D to insert ‡)**

- If materials in a language other than English are present

  - 041 _ _ ‡a lang code, repeat ‡a as needed
  
- **100:** Creator; copy and paste from finding aid
 
  - Right click > Control single heading (F11)
  - ‡d for dates, ‡c for qualifier
  - Person: 100 1 _; Family 100 3 _
  - See Michelle's documentation for forming family and other headings
  
- **245 1 0:** Title












