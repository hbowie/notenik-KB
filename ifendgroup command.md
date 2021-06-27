Title:  ifendgroup command

Tags:   levels-outline.7 Merge Templates.4 Merge Commands

Timestamp: 20210616225205

Seq:    8.4.6

Level:  4 - Subsection

Body: 

Lines following this command and preceding the next group or endif command will be written to the output file at the end of a group of records sharing a common value for this key field. 

Ifendgroup commands should follow definegroup commands and precede ifnewgroup commands, and should generally be specified in *descending* order by group number. 

The ifendgroup command has one operand.

- Group Number. The group number whose group-ending output lines follow.
