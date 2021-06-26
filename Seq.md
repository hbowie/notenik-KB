Title:  Seq

Tags:   levels-outline.6 Field Labels and Types.6 Fields for Sequencing and Outlining

Timestamp: 20210609171702

Seq:    6.5.1

Level:  4 - Subsection

Body: 

The word `seq` can be used as both a label and a type. 

In addition to `seq` itself, this field type will be inferred for field labels matching any of the following:

+ sequence
+ rev
+ revision
+ version
+ Anything beginning with `seq`

A Collection is not expected to have more than one field of type `seq`. 

A seq field is meant to contain some sort of sequence number, revision letter, version number or priority that can be used to put the Notes of a Collection into some meaningful order. 

A Seq field may contain letters, digits and one or more periods (aka decimal points) or hyphens or a dollar sign (‘$’).

You may wish to assign a unique Seq value to each Note in a Collection, but Notenik does not require this (in other words, it does allow duplicate Seq values to be assigned to different Notes).

When editing, the seq field will appear as a single line of editable text.

When displayed, the seq field will be displayed as entered.   

When used as a sort field, seq values will be padded to cause them to sort into a natural order, rather than a strict character-by-character alphanumeric order.  In other words, a value of `2` will sort before a value of `10`, a value of `b` will sort before `aa`, etc. Each segment of this field, when separated by a dot or a dash, will be padded separately.

If you'd like to see your Notes listed in sequence by their assigned number, you can use the Sort Menu to change the sequence of the displayed list from Title to Seq + Title. Use the Reverse option to see them in descending sequence. 

When adding a new Note, if the currently selected Note has a seq value, then the new Note's seq will be initialized by incrementing the selected Note's seq value. In other words, if you have your list sorted by Seq, then a new Note will be inserted immediately following the selected Note. 

If you want to insert a new note with a Seq Value already assigned to another Note, then first select the other Note, then use the Increment command under the Note menu to increment the Seq field of the existing note, as well as following notes that might otherwise cause duplicate Seq values. 

If your Notes have a two-part Seq field (i.e., 1.00), then use the `Increment Major Seq` command beneath the `Note` menu to force the numbers to the left of the decimal point to be incremented, rather than incrementing the numbers on the right.  

