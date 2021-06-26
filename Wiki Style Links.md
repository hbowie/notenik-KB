Title:  Wiki Style Links

Tags:   levels-outline.5 Markdown.1 Choice of Markdown Parsers

Timestamp: 20210607233023

Seq:    5.1.1

Level:  4 - Subsection

Index:  wiki-style links; double-bracket links; note-to-note links; 

Body: 

Notenik allows the user to create a link from one Note to another Note within the same Collection. 

In order to enable this option, the user must be using Notenik's own internal Markdown parser.

The Notenik Markdown parser supports [double-bracket wiki-style links](https://en.wikipedia.org/wiki/Hyperlink#Wikis) as an extension to the original Markdown spec from John Gruber.  

If you are using Notenik's parser, then a link to another Note may be coded by simply enclosing the title of the target Note within double square brackets, like this -- `[[Overview]]` -- and a click on the resulting link will take you to that note.

If you also enable the [[timestamp]] field for a Collection, then you can change the title of a linked Note without changing the referencing wiki link text, and Notenik will remember the association between the old title and the new title, making use of the timestamp field to preserve a unique, unchanging identity for each Note. These associations will be saved in a special file named 'alias.txt', within the Collection folder. This functionality can be useful to make sure you don't end up with broken links between Notes.




