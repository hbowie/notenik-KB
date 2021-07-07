Title:  Custom URL Scheme

Tags:   levels-outline.5 Getting Data Into and Out of Notenik.10 Custom URL Scheme

Timestamp: 20210627004934

Seq:    5.11

Level:  3 - Section

Body: 

Notenik has its own custom URL scheme, which can be invoked by other apps as a means of integrating Notenik with these other applications. 

Note that URLs must in general be [percent encoded](https://en.wikipedia.org/wiki/Percent-encoding). The most common encoding is done by replacing each space with `%20`. 

The following commands are supported.

### Open 

Following is a sample URL:  

	notenik://open?shortcut=todo&id=pickupmilk

Let's break this down:

+ `notenik://` - The custom scheme that will invoke the Notenik app. 
+ `open` - The Notenik command to open a Collection and optionally a specific Note within the Collection. 
+ `?` - A question mark indicates the end of the command and the beginning of the query string. 
+ `shortcut=todo` - The shortcut identifying the Collection to be opened. Note that shortcuts are defined in such a way that they will generally *not* need to be percent encoded. 
+ `path=Users/user1/Sites/site1` - Specifying the complete path would be an alternate way of identifying the Collection to be opened. Path values generally *will* require percent encoding. 
+ `&` - An ampersand is used to separate each `label=value` parameter from the next. 
+ `id=pickupmilk` - The ID identifying the Note to be selected for Display. Note than a Note ID is defined in such a way (removing spaces, etc.) that it will *not* need to be percent encoded. 

An easy way to obtain a complete URL that can be used to later open a specific Note is to right-click the Note's row on the List tab within Notenik, and then select `Copy Notenik URL` from the contextual menu that will pop up. This will copy a complete Notenik URL to the clipboard, from which it can then be pasted into another location. 

### Add

Following is a sample URL:  

	notenik://add?shortcut=todo&title=Pick%20up%20milk&body=You%20gotta

Again, let's break this down. 

+ `notenik://` - The custom scheme that will invoke the Notenik app. 
+ `add` - The Notenik command to add a new Note to an existing Collection. 
+ `?` - A question mark indicates the end of the command and the beginning of the query string. 
+ `shortcut=todo` - The shortcut identifying the Collection to which the new Note is to be added. 
+ `path=Users/user1/Sites/site1` - Again, specifying the complete path would be an alternate way of identifying the Collection to be used. 
+ `&` - An ampersand is used to separate each `label=value` parameter from the next. 
+ `title=Pick%20up%20milk` - The title for the new Note. This will amost always require percent encoding, as in this example. 
+ `&` - An ampersand is used to separate each `label=value` parameter from the next. 
+  `body=You%20gotta` - The body of the new Note. Again, this will almost always require percent encoding. 

Other fields may also be specified for a new Note, using a similar *label=value* convention.

### Help

Following is a sample URL:

	notenik://help?id=versionhistory
	
Once more, let's break this down:

+ `notenik://` - The custom scheme that will invoke the Notenik app. 
+ `help` - The Notenik command to open the Notenik Knowledge Base supplied with Notenik. 
+ `?` - A question mark indicates the end of the command and the beginning of the query string.  
+ `id=versionhistory` - The ID identifying the Note to be selected for Display. 

The query string is optional. If it is not supplied, then the Knowledge Base will be opened at the first Note in the Collection.