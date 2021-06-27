Title:  Level

Tags:   levels-outline.7 Field Labels and Types.5 Fields for Sequencing and Outlining

Timestamp: 20210609171814

Seq:    7.5.2

Level:  4 - Subsection

Body: 

The word `level` can be used as both a label and a type. 

In addition to `level` itself, this field type will be inferred for field labels equal to any of the following:

+ depth

A Collection is not expected to have more than one field of type `level`. 

The level field is meant to indicate each particular Note's depth within an implied tree structure made up of all the Notes in the Collection. 

A level value is represented by a single digit, and is typically restricted to the range 1 - 6. 

A level field is typically used in combination with a [[Seq]] field. 

When viewing a Collection containing a level field, and when viewing the List of Notes sorted by 'Seq + Title', the title of each Note will be indented to indicate the level of each particular Note within the implied outline. 

One way to use a level field, when generating HTML, is to generate a heading tag using the Note level as the numeric portion of the tag. 

A brief text label may also be associated with each possible numeric value. 

When editing, the level field is presented as a pick list, with the user allowed to select from the list of standard values for that Collection. 

For Display purposes, the digit and text are usually shown side-by-side. 

When used as a general sort field, level values will be sorted by their digits. 

The text values may be modified by placing a series of integer + label pairs in the Value area of the relevant template file, with separating punctuation. Such a template line might look something like this:

	Level: <level: 1 - Book Title; 2 - Section; 3 - Chapter; >
