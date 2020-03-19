# Revisions to XML

This section deals with revisions to finding aids that have already been encoded in EAD. Some may have originally been SGML documents from back in the old days of EAD. These SGML documents have now been converted to XML. Documents that started out in XML will have commented-out revision tags that you can activate. Finding aids converted from SGML won't have those commented-out tags.  

The < revisiondesc > tag in the <eadheader> is where EAD keeps track of revisions. However, the information coded in the < eadheader > section doesn't show up on the screen. Therefore, to track revision information and to make said information visible on the screen, you must enter the information in both the < revisiondesc > tags in the < eadheader > and the < processinfo > section in < archdesc >.  

In both places, how you enter the information is determined by whether or not you're the first one in with a revision.  

## Adding revision statements to < revisiondesc > in the < eadheader >: 

If you're revising an EAD-encoded finding aid that was written fairly recently, the < revisiondesc > tags for entering revision information in the < eadheader > should be the first commented-out area you encounter:  

<! -- OPTIONAL TAG: use only if revising EAD-encoded finding aid.< revisiondesc >< change >< date >Date of change</ date >< item >Updated because of ?</ item ></ change ></ revisiondesc >-- >  

If you're making the first revision to an EAD-encoded finding aid that was written when we first starting doing EAD, you may have to add the < revisiondesc > tags. Place your cursor after </ profiledesc > and before </ eadheader > and add  

</ profiledesc >  

< revisiondesc >< change >< date >(add month and year of revision)</ date > 

< item >Updated because of (say why you're updating--addition/donor request/corrections, etc.) by (your name)</ item > 

</ change ></ revisiondesc > 

 </eadheader> 
 
 If yours is NOT the finding aid's first revision (there's already a < revisiondesc > section, just add a new set of < change > tags:  

< change >< date ></ date >< item ></ item ></ change >  

## Adding revision statements to < processinfo > in < archdesc >:

You'll also need to add revision information to < archdesc > so that it will display. You needn't give a reason for revising here. You may have to turn the < processinfo > tags on or you may just be adding another to processing information already there. If the latter, you can use this template:  

< p >Revisions: Finding aid updated in < date >(add month and year of revision)</ date > by (your name).</ p >  

Here's a full-blown example of a modern < processinfo > with a revision statement:  

< processinfo >< head >Processing Information</ head >< p >Processed by: Carolyn Wallace, 1969; William Auman, 1985; Roslyn Holdzkom, 1996</ p >

< p >Encoded by: Roslyn Holdzkom, November 2003</ p > 

< p >This collection was processed with support from the National Endowment for the Humanities.</ p >< p >The Addition of November 2001 is arranged in the same way as, but has not been incorporated into, the original deposit of materials.</ p >

< p >Additions received after February 1995 have not been integrated into the original deposits. Researchers should always check additions to be sure they have identified all files of interest to them.</ p > 

< p >Finding aid updated in January 2004 by Roslyn Holdzkom because of addition.</ p > 

</ processinfo >  

Revisions can be made ad nauseam. Just keep piling them on, but feel free to do some logical consolidation of entries if things seem to be getting out of hand.  

## Adding Missing Tags

If you're revising a pre-XML EAD-encoded finding aid, you may find that some tags are missing. Three of the most common missing tags that you might want to add are available in the Other Elements section of the clip sidebar.  

### < prefercite > 

It's always a good idea to add < prefercite > if there isn't one. Add <prefercite> after < processinfo >. If there's no < processinfo >, add <prefercite> after < acqinfo >. You'll have to fill in the collection name, collection number, and edit the repository name.  

< prefercite encodinganalog="524" >< head >Preferred Citation</ head >< p >[Identification of item], in the [name of collection] #[collection number], [chose one: Southern Historical Collection, Southern Folklife Collection, University Archives, General Manuscripts], Wilson Library, University of North Carolina at Chapel Hill.</ p ></ prefercite >  

### < processinfo > 

If you need to add a < processinfo >, do so after < acqinfo >.  

< processinfo >< p >Processing Note: Enter Note.</ p ></ processinfo >  

### < accessrestrict > and < userestrict > 

You may need to add < accessrestrict > and < userestrict >. < userestrict > must follow < accessrestrict >. If there's no < accessrestrict >, add one. Add <accessrestrict> right after < head >Administrative Information</ head > and < userestrict > right after < accessrestrict >.  

< accessrestrict encodinganalog="506" >< p >Restriction: Enter Restrictions Note.</ p ></ accessrestrict >< userestrict >< p >Use Restriction: Enter Restrictions Note.</ p ></ userestrict > 

< p >Additions received after February 1995 have not been integrated into the original deposits. Researchers should always check additions to be sure they have identified all files of interest to them.</ p > 

< p >Finding aid updated in January 2004 by Roslyn Holdzkom because of addition.</ p ></ processinfo >  
