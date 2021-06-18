Title:  delims command

Tags:   levels-outline.7 Merge Templates.4 Merge Commands

Timestamp: 20210616221450

Seq:    8.4.1

Level:  4 - Subsection

Body: 

If used at all, this command should be the first command in the template file. This command overrides the standard [[Merge Delimiters]] used to indicate the beginnings and ends of commands and variables, for the remainder of the current template file. The command can have one to five operands. Each operand will become a new delimiter. They should be specified in the following order.

* beginning of a command 
* the end of a command 
* the beginning of a variable 
* the end of a variable 
* the beginning of variable modifiers 

Note that, in addition to specification of the delims command, the first characters found on the first line of the template file can trigger the Notenik template processor to use an alternate set of delimiters.
