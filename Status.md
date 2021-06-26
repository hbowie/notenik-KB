Title:  Status

Tags:   levels-outline.6 Field Labels and Types.5 Task-Related Fields

Timestamp: 20210609170808

Seq:    6.6.2

Level:  4 - Subsection

Body: 

The word `status` can be used as both a label and a type. 

A Collection should only have a single field of type `status`. 

The status field is meant to indicate a task's degree of completion, using a standard set of values. A single digit is used to place each status value into an approximate life cycle sequence. An accompanying bit of text is used to convey the human-readable meaning associated with that particular digit. 

When editing, the status field is presented as a pick list, with the user allowed to select from the list of standard values for that Collection. 

For Display purposes, the digit and text are usually shown side-by-side. 

When used as a general sort field, status values will be sorted by their digits. 

When used in a Task sort, status values will be converted to an `X`, for any numeric value greater than or equal to 6, or a space, for any value less than 6. The intent is to sort completed tasks to the bottom of a list sorted in this fashion. 

Notenik will default to the following standard list of status values.  

* 0 - Suggested
* 1 - Proposed
* 2 - Approved
* 3 - Planned
* 4 - Active
* 5 - Held
* 6 - Completed
* 7 - Pending Recurs
* 8 - Canceled
* 9 - Closed

The text values may be modified by placing a series of integer + label pairs in the Value area of the relevant template file, with separating punctuation. Such a template line might look something like this:

	Status: 1 - Idea; 4 - In Work; 9 - Published;

See these commands beneath the Note menu. Note that these are designed to be used in Display mode, not in Edit mode. 

* Toggle Status - Switches from least complete to most, and back again. 
* Increment Status - Bump to the next stage in the Collection's lifecycle. 

There's also a command beneath the Collection menu to Close all Completed Tasks, which will look for all tasks with a status of Completed and change them to Closed. 

Look under the File menu for an option to Purge Notes that have been Canceled or Completed. You'll be given the option of discarding the purged Notes, or of copying them to another location.
