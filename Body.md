Title:  Body

Tags:   levels-outline.6 Field Labels and Types.4 The Basic Set of Fields

Timestamp: 20210609165933

Seq:    7.4.4

Level:  4 - Subsection

Body: 

The word `body` can be used as both a label and a type. 

A Collection must have one and only one field of type `body`, and it should be the *last* field within a Collection. 

The body field consists of free-form text: in other words, this is the stuff that would colloquially be considered a *note*. 

When parsing a Notenik text file, the body field has the special distinction of allowing the inclusion of lines that might otherwise be interpreted as additional fields (since Notenik knows that no other legitimate field definitions are allowed to follow the body entry). 

When editing, the body field will appear as a multi-line text field, and will take up whatever available space is left after  the edit widgets for other fields have been presented. 

For Display purposes, the body field will be run through a Markdown parser before presentation.
