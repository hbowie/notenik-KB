Title:  Input Module Parameters

Tags:   levels-outline.8 Script Files.2 Scripting Modules

Timestamp: 20210617211315

Seq:    8.2.1

Level:  4 - Subsection

Body: 

The action for an input command may be either 'set' or 'open'. The set command(s) should precede the open command to which they will apply. 

#### Set

When using 'set', the variable to be set would be named in the object column, and the value to which it should be set would be supplied in the value column. 

The following variables may be set.

* xpltags - Set this variable to 'true' to create a row for each tag included in the original row's Tags field. A field called 'Tag' will be added to the data source. Set the variable to 'false' to bypass tags explosion. 

* dirdepth - The number of levels of folders to be considered, when reading from a data source that might drill down into multiple folders. The top level folder specified counts as 1. 

#### Open

When using 'open', the modifier field specifies the type of data source, and the value field specifies a path to the data source to be opened. 

The object field is normally left blank, but an object of 'merge' can be used to cause the current data source to be merged with the prior data source, rather than replacing it. 

The following modifier values are valid:

* dir - Reads the directory entries from the specified directory (including sub-directories, if the dirdepth variable has been set to a value greater than 1).

* file - Reads an input text file with columns separated by tabs or commas. 

* markdown-with-headers - Reads a Markdown-formatted text file, and chunks it up into sections based on its headers. The content of each header will be placed in the Title field, the level of each header (1 - 6) will be placed in a Level field, and all text between this header and the next one will be placed into the Body field.

* notenik-defined - Reads a Notenik collection with its fields defined by a template file. 

* notenik+ - Reads a Notenik collection with a broad set of standard fields. 

* notenik-general - Reads a Notenik Collection with any set of fields. 

* notenik-index - Reads a Notenik Collection using the Index field, and generates one row for each index term, containing the following columns. 

	- Initial Letter - The first letter of the index term. 
	- Term - The term being indexed. 
	- Lower Case Term - The same index term, but converted to lowercase.
	- Term Link - A definitive link that has been supplied for this term. 
	- Page - The Title of the Note containing this index term. 
	- Page Type - The Type of the Note containing this index term. 
	- Anchor - 

* notenik-split-tags - Reads a Notenik Collection, adds a "Tag" field, and returns one row for each tag (or one row with a blank tag, for Notes with no tags). 

* xlsx - Reads the first table in the specified XLSX file. 


