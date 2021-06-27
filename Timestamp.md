Title:  Timestamp

Tags:   levels-outline.7 Field Labels and Types.10 System-Assigned Dates and Times

Timestamp: 20210609175521

Seq:    7.10.3

Level:  4 - Subsection

Index:  zettelkasten; 

Body: 

The word `Timestamp` can be used as both a label and a type. 

A Collection should never have more than one field of this type. 

This field is assigned when a Note is first created, and is an alternate means of identification for a Note that will persist even if the title of the Note is later changed. 

Timestamp values will be generated in a "yyyyMMddkkmmss" format, consisting of:

* 4-digit year
* 2-digit month
* 2-digit day of month
* hour of day, using a 24-hour range
* minute of hour
* second of minute

All of this is normalized to Greenwich Mean Time, and formatted without spaces or punctuation. 

This field is system-maintained, and is not editable by the user. 

The field is generally displayed below all user-editable fields, and may be separated from these other fields by a divider. 

The values for this field can be exported and imported, and will then serve the purpose of preserving an original value for this field, rather than reflecting the date and time of the import.

Timestamps such as these are often used when creating a *[zettelkasten](https://zettelkasten.de)*.

A timestamp field is particularly important when you are using [[Wiki Style Links]] within a Collection. 

If you enable the timestamp field for a Collection, then you can change the title of a linked Note without changing the referencing wiki link text, and Notenik will remember the association between the old title and the new title, making use of the timestamp field to preserve a unique, unchanging identity for each Note. These associations will be saved in a special data store for the Collection. This functionality can be useful to make sure you don't end up with broken links between Notes.
