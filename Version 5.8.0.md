Title: Version 5.8.0 

Tags:  

Link: 

Timestamp:  

Seq: 10.8 

Level: 3 - Section 

Index:  

Body: 

Released on 28 Mar 2021
 
##### Fixed a Bug that was resulting in a double descending sort

When sorting via the Scripting module, the sort was honoring both the direction specified in the script commands, as well as the direction specified most recently in the Collection preferences. If both were set to descending, then the result would be a double-negative, resulting in an ascending sort. This has been fixed. 

 
##### Added Page Type as an additional column for notenik-index scripting input

If the Collection has a Type field, then this will appear in the Page Type column generated when using the notenik-index scripting input type. 

 
##### Tweaked the Linked Tags Template Variable Modifier

One or more CSS classes can now be specified, to be applied to the link generated for each tag. These should be specified following the path, with an intervening semicolon to separate the two. 

 
##### Added an Author Name Variable Modifier

Use the letter "A", followed by a "1" or a "2", to replace the full name with the last name only, or with the last name first, followed by a comma and the first name. 

 
##### Added copyfile template command

A `copyfile` command can now be used, as part of a merge template, to copy an accompanying file (typically an image file identified by the new Image Name field) to an appropriate output destination, from which it can be accessed by an output web page. 

 
##### Added Image Name field label and type

The user can now specify the name to be associated with a Note, by selecting from a list of available attachments. 

 
##### Added Minutes to Read field label and type

The value will be calculated automatically, based on the number of words found in the body field, figuring 200 words per minute, then rounding to the nearest whole number. 

 
##### Refactoring of file input/output routines

Extensive refactoring of file input and output routines to isolate actual interactions with the file system. 

