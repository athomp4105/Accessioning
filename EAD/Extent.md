# Extent (overriding "approximately")

Usually extent coding looks like this: 

```
<physdesc label="Extent">

<extent unit="items" encodinganalog="300">7000</extent> 

<extent unit="linear feet" encodinganalog="300">5.0</extent> </physdesc> 
```
 

If you have an exact item count and want to override "approximately" in the extent statement: 

Remove unit="items" from the first extent statement AND the entire second extent statement. Add the linear feet as a parenthetical after the item count. 

 

Code like this: 

```
<physdesc label="Extent"> 

<extent encodinganalog="300">6990 items (5.0 linear feet)</extent> </physdesc> 
```
