Title:  System Variables

Tags:   levels-outline.8 Merge Templates.2 Merge Variables

Timestamp: 20210610152725

Seq:    8.2.1

Level:  4 - Subsection

Body: 

The following special variables are predefined and available for substitution, no matter what data source is being used.

datafilename
: The name of the data source being used.

dataparent
: The path to the enclosing folder for the current data file. This can be used as part of an output command to specify an output file in the same folder as the data file.

nobr
: Placing the variable 'nobr' anywhere on a line will cause that line to be written out without a trailing line break. The nobr variable itself will be removed from the line, without being replaced.

parentfolder
: The lowest-level folder immediately enclosing the data file.

relative
: If a Web Root directory has been specified, then this variable will be replaced by the relative path from the output file being created back to the root directory.

templatefilename
: The name of the template file (not including the path to the template file).

templateparent
: The entire parent path to the template file, excluding the file name itself.

today
: The current date, at the time that template output is being generated.
