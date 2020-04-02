# Headings for archival records (authority work)

## Contents

- Family names as creators
- Authority records for family names
- Family names as subjects
- Searching for the authority file
- Personal name headings
- Subject headings

## Family names as creators

When used as creators, family names should have qualifiers added to differentiate them from other families of the same name. 

Some examples from the authority file: 

- Johnson (Family : ǂg Johnson, Benjamin F. (Benjamin Franklin), 1818-1905) 
- Johnson (Family : ǂd 1804-1962 : ǂc Me.) 
- Jones (Family : ǂd 1797- : ǂc South Carolina) 
- Smith (Family : ǂg Smith, Upton Treat, 1843-1925) 

**RDA 10.11** covers the rules for constructing family names.  You’ll always start with the name of the family, with (Family) in parentheses following the name, followed by any other qualifiers. 

The other qualifiers that can be used are as follows:

- Dates associated with the family, in **$d**
- Place associated with the family, in **$c** 
- Prominent member of the family, in **$g**.  The name should be given in inverted order, last name first, in the same form that the person is established in the authority file or given as a heading in your record, except that any MARC coding will be removed within the **$g**. 

Family names as creators will be coded **100 3_ or 700 3_** in the MARC record. 

## Authority records for family names

In the family name authority record: 

- 376 Families ǂ2 lcsh 
- 376 ǂb [name of progenitor, if in the 100] ǂ2 naf 
- 500 1_ ǂw r ǂi Progenitor: ǂa 
- 500 1_ ǂw r ǂi Family member: ǂa   

In related personal name authority records: 

- 500 3_ ǂw r ǂi Descendants: ǂa 
- 500 3_ ǂw r ǂi Family: ǂa 

## Family names as subjects

The types of heading described above for family names as creators are not eligible to be used as subjects.  Family names as subjects will just be in the form “Smith family” or “Jones family,” with no added qualifiers.  These should be coded as **600 34**: 

- 600 34 Cameron family. 
- 600 34 Battle family. 

Using second indicator **4** (source not specified) instead of second indicator **0** (Library of Congress subject headings) will prevent the authority vendor from flipping unauthorized family names to their authorized forms. 

## Searching the authority file

You can search the LC authority file for names and subjects at http://authorities.loc.gov/.  Choose Subject Authority Headings or Name Authority Headings, as appropriate.  Both personal and corporate names are searched under Name Authority Headings.  Subject Authority Headings is for topical headings. 

## Personal name headings

Say you want to find the authorized heading for the musician Paul Brown.  Search by last name, first name in the authority file and you get this (plus many more). 

![screenshot](https://user-images.githubusercontent.com/58087302/78273256-9a629300-74dc-11ea-82b3-2d78b355af8e.png "Brown personal name headings 1")

You may know that Paul Brown was born in 1952 and be able to jump down to this part of the list: 

![screenshot](https://user-images.githubusercontent.com/58087302/78273750-47d5a680-74dd-11ea-8bd7-ed61e3b9ae2d.png "Brown personal name heading 2")

Click on the red button to the left of each heading and you’ll eventually be taken to the authority record (for some reason this requires many more steps than it should), which should give you an idea of whether or not each person is likely to be the one you want.  Some authority records have a lot of information and some have very little.  The record for Brown, Paul, 1952- looks like this: 

![screenshot](https://user-images.githubusercontent.com/58087302/78273911-6fc50a00-74dd-11ea-9181-dc22688eea3f.png "Brown personal name heading 3")

So this looks likely to be the person represented in an SFC collection.  You’ll copy the form that appears in the 100 field and use that in your finding aid.  Any 400 fields are cross-references that are there to lead you to the 100 field.  500 fields are see also references that link two related entities that are both established (e.g., John Lennon and the Beatles). 

If you’re searching a common name and you don’t want to go through the whole list of records in the authority file, a shortcut can be to start in our local catalog.  If the person is a folk musician, you can search on their name and limit to SFC as a location and possibly find the correct heading that way.  But, remember!  Once you’ve found a heading, make sure you go back to the LC authorities site and pull up the authority record there to make sure the heading is for the right person.  We have plenty of incorrect name headings in our catalog that don’t match the authority file, so we can’t blindly follow what is in the UNC catalog and assume that it’s correct. 

So, what do you do if you can’t find an authority record for the person you’re looking for?  In that case, you can construct your own heading, but you have to make sure it is different from any established headings in the authority file, and that it’s consistent with headings used already in the UNC catalog.  If you don’t find anything in the authority file, you should search the UNC catalog (preferably the classic catalog, http://www2.lib.unc.edu/webcat/, which is better for doing this kind of search) to see if the person has appeared already in our catalog, and if so, copy the form found there. 

If there’s nothing in either the authority file or the UNC catalog, you can formulate a name heading—usually last name, first name, with birth and/or death dates if available.  

Examples:     

- Larman, Howard.
- Michal, William Norwood, Sr., 1906-1991.

If you don’t have any dates to use to differentiate someone with a common name, you can add a qualifier in parentheses.  

Examples: 

- Cohen, Mike (Guitarist)
- Adams, Nicholas (Photographer)

A note on the form of name headings—the authority file is wildly inconsistent in how people are established.  Some people get the full birth date, death date, middle name treatment (e.g., Ashe, Samuel A. (Samuel A'Court), 1840-1938) while others have very simple headings (e.g., Haggard, Merle).  As a general rule, birth and death dates are added if they’re readily available at the time the authority record is created or they’re needed to differentiate, but otherwise they aren’t included, even if the person goes on to become very famous—we don’t go back and add dates once a heading is established. 

In some cases, a person gets established under the name used on their first published work, and then they go on to use a different name predominantly.  Generally, once a heading is established it isn’t changed (though it can be under some circumstances).  We’ll usually just add 400 fields as cross-references from any other forms of name that someone might search under.  

So all this is to say that the way someone is established in the authority file might not be ideal, but we have to use that form regardless. 

## Subject headings

Say you want to add a subject heading about cooking, and you vaguely remember that the word “Cookery” was used for this concept in the past.  You might search “Cookery, American,” and get the following result: 

![screenshot](https://user-images.githubusercontent.com/58087302/78275344-7d7b8f00-74df-11ea-96ce-2d17d9094d0a.png "Cookery subject heading 1")

Do not just copy the heading found in this list into your record!  You need to open up the authority record and make sure that (1) you’re choosing the authorized form (rather than a cross reference), and (2) the heading is actually for a subject and not something else.  The authority file also includes records for things like series headings, which might look like subjects but are actually not. 

The “References” button next to Cookery, American, is a clue that this is actually a cross-reference and not an authorized heading.  Clicking on this button will lead you to the authority record, which looks like this: 

![screenshot](https://user-images.githubusercontent.com/58087302/78275865-3346dd80-74e0-11ea-9436-a2c5207b0c2b.png "Cookery subject heading 2")

Thus, “Cooking, American” is the authorized heading, because it’s in the 150 field.  “Cookery, American” is a superseded form of the heading.   

It’s also okay to copy subject heading strings that you find in the UNC catalog.  For more complicated headings with subdivisions, this will be much easier than searching the authority file.

For instance:

- Roads—North Carolina—Mecklenburg County—Design and construction. 
- University of North Carolina (1793-1962)--Students--Photographs. 

