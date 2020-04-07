# Find and Replace with Regular Expression

Using Regular Expression in Oxygen to create a **POWERFUL & SMART** “find and replace” search string:  

From time to time while processing, we have all come across changes that need to be made to the EAD that only effect the tags we are using, not the metadata between the tags.  

Example:

**Take→**

![Initial record with tags that require changes to the code](https://user-images.githubusercontent.com/58087302/78701037-50aaeb80-78d4-11ea-9431-9e1275d6c43a.jpeg "Example needing change")

**Change it to→**

![Changed record with improved tags](https://user-images.githubusercontent.com/58087302/78701232-abdcde00-78d4-11ea-8f50-06546165d184.jpeg "Example with changes")

In this example, I want to **remove the ```<emph render=”doublequote”>``` from the scope content notes (Location and Photographer) but NOT from the ```<unittitle>```**. In this particular finding aid, there are tens of thousands of entries; each with different locations and photographers. Add to it that I **don’t want to touch the other ```<emph render=”doublequote”>``` tags in each entry.** The solution is using the REGULAR EXPRESSION feature available in the Oxygen “Find and Replace” feature. First, let me state: I AM NOT A PROGRAMMER in any sense of the word, but I have spent the last few years learning about Python and Regular Expression and how they can be used to navigate the world of EAD/XML especially in regards to the creation of POWERFULL search features.  

I will show how to use Regular Expression within Oxygen to make the changes shown above.  

1. Open the .xml you are going to be making the changes to in Oxygen.  

2. Find an example of the metadata that needs to be changed within the .xml file 

**See Example→**

![Highlighted text](https://user-images.githubusercontent.com/58087302/78701716-7dabce00-78d5-11ea-8ad1-3c0f981f43b2.jpeg "Example within instructions 1")

3. Select “Find” from options at top of window and select “Find and Replace” 

4. Under “Options” check “Regular expression” and “dot matches all”  

**See Example→**

![Windowed text 1](https://user-images.githubusercontent.com/58087302/78702032-f3179e80-78d5-11ea-841a-d831f578122f.jpeg "Example within instructions 2")

In this case, what I want to do is strip out the ```<emph render=”doublequote”>``` and ```</emph>``` tags from the scope content portion and nowhere else. In this case, all of the tags I am looking to replace are nested in "p" tags found within the scopecontent feature. This is a great use for regular expression.  

Simply put, Regular Expression is a set of special (predefined) characters that can be used to parse stings of characters and identify patterns. It is more complex than that, but for our purposes, this is good. (There are lots of sites out there but check out : http://www.regular-expressions.info/reference.html)  

5. Here is how the find and replace should be formed: 

**See Example→**

![Windowed text 2](https://user-images.githubusercontent.com/58087302/78702221-40940b80-78d6-11ea-8d35-b7ff6f07918e.jpeg "Example within instructions 3")

In the example above: In “Text to find” there are two uses of regular expression:  

- “ **.*?** ” → In this example, this is RE (Quantifier) for “everything in-between” the tags  
- “ **( )** “ → In this example, this is RE (Range) for “keep this string together”  

In the “Replace with” there is one use of regular expression:  

- “ **$1** ” → In this example, this is RE (String Replacement) that inserts whatever was “kept together” in the “Text to find” (above in find and replace)  

Created by Patrick Cullom.
