# EAD

All AV materials are coded at the item-level - even materials that span multiple tapes or reels.  

Below is information on how to code an AV item at a minimum and moderate level. 

## Minimum (Required):

```
<did> 

<container type="container type">Call Number</container> 

<unittitle>Title</unittitle> 

<physdesc> 

<genreform>Format</genreform> 

</physfacet> 

</did> 
```

## Moderate:

```
<did> 

<container type="container type">Call Number</container> 

<unittitle>Title</unittitle> 

<physdesc> 

<genreform>Format</genreform> 

<extent> Reel Size (audio) / Duration (video) / Length in feet (film)</extent> 

</physfacet> 

</did> 
```

Below are examples of how to code an audio, video, and film item when additional information is available. In general, try to keep description at a minimum. 

### Audio

```
<did> 

<container type="sfcaudioopenreel">Call Number</container> 

<unittitle>Title, <geogname>Place</geogname>, <unitdate>Date</unitdate>: tape number</unittitle>     

<physdesc> 

<genreform>Format</genreform> 

<extent> Reel Size ; Speed ; Duration </extent> 

<physfacet>element type</physfacet> 

</physdesc></did> 

<scopecontent> 

<p>Content Description - abstract, song titles, credits, etc</p> 

</scopecontent> 

<processinfo><p>Processing info - previous numbering schemes, pointing to field notes or related items, playback issues, etc.</p></processinfo> 
```

#### Audio Example:

```
<did> 

<container type="sfcaudioopenreel">FT-20009/1</container> 

<unittitle>Mike and Alice, <geogname>Atlanta, Ga.</geogname>, <unitdate>Date</unitdate>: tape 1 of 2</unittitle>     

<physdesc> 

<genreform>1/4” Open Reel Audio</genreform> 

<extent>5" reel ; 7.5 ips ; 15 minutes, 20 seconds</extent> 

<physfacet>original</physfacet> 

</physdesc></did> 

<scopecontent> 

<p>Recording of Mike Seeger and Alice Gerrard performing live.</p> 

</scopecontent> 
```

### Video

```
<did> 

<container type="videotape">Call Number</container> 

<unittitle>Title, <geogname>Place</geogname>, <unitdate>Date</unitdate>: tape number</unittitle>   

<physdesc> 

<genreform>Format</genreform> 

<extent>Duration</extent> 

<physfacet>element type ; color/black and white ; silent/sound (sound type)</physfacet> 

</physdesc></did> 

<scopecontent> 

<p>Content Description - abstract, song titles, credits, etc</p> 

</scopecontent> 

<processinfo><p>Processing info - previous numbering schemes, pointing to field notes or related items, playback issues, etc.</p></processinfo> 
```

#### Video Example:

```
<did> 

<container type="videotape">VT-20009/1</container> 

<unittitle>Elizabeth Cotton, <geogname>Chapel Hill, N.C.</geogname>, <unitdate>1983</unitdate>: tape 1 of 2</unittitle>   

<physdesc> 

<genreform>Betacam SP</genreform> 

<extent>30 minutes</extent> 

<physfacet>edited master ; color ; sound (mono)</physfacet> 

</physdesc></did> 

<scopecontent> 

<p>An interview with Elizabeth Cotton conducted by Mike Seeger.</p> 

</scopecontent> 

<processinfo><p>Memo found with original container resides in Folder 3</p></processinfo> 
```

### Film

```
<did> 

<container type="film">Call Number</container> 

<unittitle>Title, <geogname>Place</geogname>, <unitdate>Date</unitdate>: reel number</unittitle> 

<physdesc> 

<genreform>Format</genreform> 

<extent>Length (feet) (Duration)</extent> 

<physfacet>element type ; color/black and white ; silent/sound (sound type)</physfacet> 

</physdesc></did> 

<scopecontent> 

<p>Content Description - abstract, song titles, credits, etc</p> 

</scopecontent> 

<processinfo><p>Processing info - previous numbering schemes, pointing to field notes or related items, playback issues, etc.</p></processinfo> 
```

#### Film Example:

```
<did> 

<container type="film">F-20009/1</container> 

<unittitle>Alice and Hazel, <geogname>Chapel Hill, N.C.</geogname>, <unitdate>1973</unitdate>: reel 1 of 2</unittitle> 

<physdesc> 

<genreform>16mm motion picture film</genreform> 

<extent>800 ft. (25 minutes)</extent> 

<physfacet>reversal ; color ; sound (magnetic)</physfacet>  

</physdesc></did> 

<scopecontent> 

<p>Footage of Alice Gerrard and Hazel Dickens performing live.</p> 

</scopecontent> 
```

### Born-Digital AV

```
<did> 

<container type="digfolder"> 

<extref href="[insert cdr link]"Call Number</extref></container> 

<unittitle>Title, <geogname>Place</geogname>, <unitdate>Date</unitdate></unittitle> 

<physdesc> 

<extent>Number of files</extent> 

</physdesc></did> 

<scopecontent> 

<p>Content Description - abstract, song titles, credits, etc</p> 

</scopecontent> 

<processinfo><p>Processing info - source media, date of original files, note regarding access copies, etc</p></processinfo> 
```

#### Born-Digital Example:

```
<did> 

<container type="digfolder"><extref href="https://cdr.lib.unc.edu/list/uuid:b699afe5-17e3-4020-a55b-a4746c0353f7">DF-20469/1</container> 

<unittitle>Fiddler's Grove Bluegrass Festival, <unitdate>1973</unitdate></unittitle> 

<physdesc> 

<extent>1 digital file</extent> 

</physdesc></did> 

<scopecontent> 

<p>An edited digital version of Brian Burch's Super 8mm footage (F-20469/1-9) set to traditional music. Edited by Brian and Gillen Burch.</p> 

</scopecontent> 

<processinfo><p>Processing information: The digital files were extracted from DVD. Original DVD files are dated 6 July 2005. An access .mp4 file was made from the DVD files for viewing purposes.</p></processinfo> 
```
