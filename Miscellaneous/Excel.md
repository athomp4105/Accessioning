# Excel formulas/tips

### Deleting empty cells

Home tab-->Find & Select-->Go to Special...-->Blanks 

Home tab-->Delete-->Delete cells 

### Breaking apart strings of text

Delimit by characters (will delimit by every instance of this character within the string) 

   Data tab-->Text to Columns-->Delimit-->Choose your delimiters 
   
By Formula (can delimit by only first instance of character) 

```
=LEFT(A1,FIND("[delimiter]",A1)-1)  

=RIGHT(A1,LEN(B1)-FIND("[delimiter]",A1)) 
```
 
**Example:**

T-40328/1 Mix 1  in column A 

To break apart by first space so you can have "T-40328/1" in one column and "Mix 1" in another, use  

```=LEFT(A1,FIND(" ",A1)-1) and =RIGHT(A1,LEN(B1)-FIND(" ",A1))``` 


