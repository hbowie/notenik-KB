Title:  output command

Tags:   levels-outline.7 Merge Templates.4 Merge Commands

Timestamp: 20210616224608

Seq:    7.4.3

Level:  4 - Subsection

Body: 

This command names and opens the output file, where the results of the template merge will be stored. The single operand is the name of the output file. This command would normally be the first line in your template file. Subsequent template records will be written to the output file.

Note, however, that the filename can contain a [[Merge Variable]]. In this case, the output command would follow the [[nextrec command]], and a new output file would be opened for each row input.

