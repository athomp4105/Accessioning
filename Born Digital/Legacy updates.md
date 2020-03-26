# Legacy updates to finding aid

1. Update revision description:

   - Insert change tags between revisiondesc tags: 

   ```<change> <date>[Month] 2015</date> <item>Finding aid updated for born digital processing by [Name].</item> </change>```

   - Some finding aids might not have revisions description tags. Insert revisiondesc tags between profiledesc and eadheader: ]

   ```</profiledesc> <revisiondesc> </revisiondesc> </eadheader> ```

2. Update processing info:

   ```
   <processinfo> <head>Processing Information</head> 

   <p>Finding aid updated for born digital processing by [Name], [Month] 2015. </p> </processinfo> 
   ```

3. Update items seperated:

   - Remove description of the physical item (FD-, DVD-, DCD-, etc.)  

   - List as Digital Folder (DF-): 

   ```<separatedmaterial> <head>Items Separated</head> <list type="simple"> <item>Digital Item (DF-40124/1) available in the Carolina Digital Repository. </item> </list> </separatedmaterial>```

4. Add an item-level note explainging the files came from legacy media:

   ```<c03> <did> <container type="digitem"><extref href="https://cdr.lib.unc.edu/list/uuid:fb046a55-7424-4092-87cf-94af90d054eb">DI-40124/1</extref></container><unittitle>North Carolina Fellows Program: <emph render="doublequote">Perspectives on Diversity</emph></unittitle> </did> <scopecontent> <p>Produced by the Class of 2005.</p><p>Migrated from DVD-40124/1.</p> </scopecontent></c03> ```

## In the CDR:

1. Update the MODS:

   - **Title:** Should be the same as the digital item/folder title in the finding aid.

   - **Identifier:** Should be the same as the item/folder number

   - **Example:** DF-40124/1
 
   - **Note:** Add a note explaining the files were migrated from original media

2. Move folders out of unprocessed.

3. Publish items.
