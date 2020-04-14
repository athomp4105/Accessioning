# Creating collection level records

1. Make sure you're on your branch in sourcetree. 

2. Login to unctechservices@gmail.com and navigate to the backlog folder. Find a backlog ticket not marked as "done." 

3. Open the backlog tracking spreadsheet, located in departmental document in sharepoint. Add the collection information into the tracking sheet. 

4. In oxygen, open the flasher template for the right Collection (SFC, SHC, UA). Templates are located here: G:\wilson\ts\archival\CLR_templates 

5. With the template open in oxygen, save the file in the git repo as the collection number. Save as-->navigate to C:\Users\[username]\Documents\finding-aids\[Collection]-->save as [collection number].xml.  

   For example, if you're working on a SHC collection, you should have the file saved as the collection number (ex. 05678.xml) under C:\Users\[username]\Documents\finding-aids\SHC. When saved here, "uncommitted changes" should show up at the top of your log/history on your branch in sourcetree. 

6. Follow the find-and-replace flasher directions at the top of the xml file with the information provided in the ticket. When done, delete flasher directions. 

7. Fill out the creator, extent, and abstract. Add a bio/hist and scope/content if included in the ticket. 

   - Creator could use ```<persname>```, ```<corpname>```, or ```<famname>``` depending on type of creator. 
   
   - You may only be given one form of extent (item count or linear feet). If so, just include it in the correct tags and comment out the other field. 
   
   - Please keep "Acquired as part of..." sentence at the end of the abstract. 
   
   - If including a bioghist note, change the header to either Biographical or Historical depending on the type of note. E.g.
   
     ```<head>Biographical/Historical Note</head> becomes <head>Biographical Note</head> ```
     
8. Transform the file and check everything over. 

9. Commit/push your changes on your branch in sourcetree. 

10. Label the email ticket as "Done." 

11. Mark x under "collection level finding aid" for the collection in the backlog tracking spreadsheet.  


