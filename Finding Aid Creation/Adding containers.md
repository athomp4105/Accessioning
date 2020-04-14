# Adding container lists to existing collection level records

1. In Sourcetree, make sure you're on the right branch. 

2. Open Oxygen. Open the xml file you need to edit from the finding aid repository 

   (Users\username\Documents\finding-aids). File name = collection number. 

3. Make sure the url in the header (line 3) is **https**, and not **http**. 

4. Remove type="unprocessed" from the accessrestrict tag. 

   - ```<accessrestrict type="unprocessed">``` becomes just ```<accessrestrict>```
   
   - Unless there are restrictions on the collection, remove the restriction note within the ```<p>``` tags and replace with ```<p>No restrictions. Open for research.</p>```
   
5. Add identity to the abstract if you can make a reasonable assumption. 
   
6. Remove the comment out tags (```<!-- -->```) from the userestrict. Should read ```<p>No usage restrictions.</p>``` unless restrictions apply. 
   
7. Remove the comment out tags from acqinfo and include acquisitions information and accession number within the ```<p>``` tags. 
   
   Example:
      
   ```
   <acqinfo encodinganalog="541"> 

   <head>Acquisitions Information</head> 

   <p>Received from John Smith in April 2019 (Acc. 123456).</p> 

   </acqinfo> 
   ```

8. In ```<processinfo>```, remove the summary description (This summary description was created...), and replace with <p>Processed by [your name], [month year] 

   - Add ```<p></p>``` tags, and put the identity statement between them. 
   
     ```<p>Since August 2017, we have added ethnic identities for individuals and families represented in collections. To determine ethnic identity, we rely on self-identification; other information supplied to the repository by collection creators or sources; public records, press accounts, and secondary sources; and contextual information in the collection materials. Omissions of ethnic identities in finding aids created or updated after August 2017 are an indication of insufficient information to make an educated guess or an individual’s preference for ethnicity to be excluded from description. When we have misidentified, please let us know at wilsonlibrary@email.unc.edu.</p>``` 

9. Add container list under ```<head>Detailed Description of the Collection</head>

   - Remove the coment out tags.
   
   - Remove "Enter Description Information Here" and replace with container list.
   
   - Start with ```<c01>``` tags.
   
     ```
     <c01 level="collection"> 

          <did><unittitle>[collection title, collection dates]</unittitle></did> 

     </c01> 
     ```

   - Add ```<c02>``` tags for each container listing, between ```</did>``` and ```</c01>```
   
     ```
     <c01 level="collection"> 

          <did><unittitle>[collection title, collection dates]</unittitle></did> 

          <c02><did><container type="[container type]">[Container number]</container><unittitle>[Box/folder title]</unittitle></did></c02> 

     </c01> 

   - Refer to container type list under the EAD tab of the notebook for valid container types and how to write container numbers. 

   - Clean up container title capitalization, etc. 

10. Optional tags:

    - ```<scopecontent><p>[Scope/content note]</p></scopecontent>```
   
      - Use for notes about content of the container that's not in the title. Goes between ```</did>``` and ```</c02>```
      
    - ```<accessrestrict><p>[Restriction note]</p></accessrestrict>```
    
      - Use for restrictions on containers. Goes between ```</did>``` and ```</c02>```
      
    - For titles that need to be in italics, use ```<title render="italic">[Title]</title>```
    
    - Copy/paste any diacritics. 
    
11. Transform the xml file to check your work. In Oxygen, click on the wrench with the red triangle, select your transformation scenario, and apply associated. The transformation should load in your default browser. 

12. Save changes in Oxygen.  

13. On your branch in Sourcetree, you should see "uncomitted changes" at the top of the log/history. Click on File Status and stage the file to commit. In the comment field, add a comment with [Collection number]: [brief description of changes made], then click commit. Keep the "push changes immediately" box checked. If Sourcetree tells you there are changes to push after you've committed, click the push arrow (but make sure you're on your branch first!)  

14. Fill out a blue sheet and give to Laura Smith when you're done.  




