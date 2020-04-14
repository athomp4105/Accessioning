# Mechanics

## Acquisition Information

Include all accession numbers for processed materials at the collection level. 

**For additions:** Also include RT and Acc. Numbers in Acquisitions Info tags at the series, file, or container levels, using the label “Acquisitions Information.” 

## Dates

Date ranges cover entire collection, series, etc.  

Make collection dates consistent in the following tags: 

```
<titlestmt> <titleproper encodinganalog="title"> 

<frontmatter> <titlepage> <titleproper> 

<unittitle label="Title" encodinganalog="245"> 
```

## Extent

Check the math across series to ensure that extents add up. Rounding up or down is okay. 

For additions: add addition extent to collection extent. 

## Subject Headings

Be sure to include a headings for the creator

## Items Separated

Include all materials housed separately in the stacks and stored digitally. 

For additions: Check existing numbering. 

## Processing and Revision Notes

Update when making revisions to existing finding aids. In the revision note, also record the last folder/format numbers used: 

```
<processinfo></processinfo> (viewable to public) 

<revisiondesc><change> <date></date>Updated for 
addition of DATE (Acc. XXXXXX) by NAME. Last folder
(1001); imagefolder (PF-XXXXX/22; oversize folder 
(OF-XXXXX/38)<item></item> </change><revisiondesc> 
```

## Related Collections

List relevant related collections. Hyperlinking other UNC collections is now possible (example below).  

```<item><extref href="http://finding-aids.lib.unc.edu/20386/">Ken Griffis Collection (#20386)</extref></item>```

## Restrictions

Check control files & AT. 

Note at every level—collection, series, and container. 

Remove outdated restrictions and “This collection contains unprocessed…”, if applicable. 

## Special Characters

Code ampersands ```&amp;``` 

Do not use curly quotes and/or apostrophes.  

Check for funky characters in the html. 

Add the statement about diacritics if appropriate. 

**Diacritics and other special characters have been omitted from this finding aid to facilitate keyword searching in web browsers.** 

[From](https://adminliveunc-my.sharepoint.com/personal/ljcb_ad_unc_edu/Documents/Checklist%20Mockup.docx)
