Title: Version 5.9.0 

Tags:  

Link: 

Timestamp:  

Seq: 10.6 

Level: 3 - Section 

Index:  

Body: 

Released on 10 May 2021
 
##### Merge Templates No Longer Write Unmodified Files

Before writing an output file from a Merge Template operation and overwriting an existing file, Notenik will now first read the existing file, and compare it to the file about to be written. If the contents are identical, then Notenik will skip the write operation. This helps to preserve last modified dates, which in turn helps to prevent unnecessary FTP operations when updating a website. 

 
##### Added New Customization Options for the Display Tab

The layout and appearance of the Display tab can now be modified by supplying a `display.css` file within a Notes Collection, or by supplying a `display.html` template file. 

 
##### Added allfields command to Merge Templates

The `<?allfields?>` command can now be used to insert all of the fields from an input record/note into the output, formatted into HTML in the same way that they would be on the Display tab within Notenik. 

