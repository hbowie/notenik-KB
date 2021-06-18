Title:  Merge Commands

Tags:   levels-outline.7 Merge Templates.4 Merge Commands

Timestamp: 20210616221125

Seq:    7.4

Level:  3 - Section

Body: 

All commands must be enclosed in the chosen [[Merge Delimiters]]. In addition, all commands must appear on lines by themselves. Command names can be in upper- or lower-case. Each command may have zero or more operands. Operands may be separated by any of the following delimiters: space, comma (','), semi-colon (';') or colon (':'). Operands that contain any of these delimiters must be enclosed in single or double-quotation marks.

The following commands are recognized. They are presented in the typical sequence in which they would be used.

<div class="pnobr">
<p>&lt;?delims new delimiters?&gt;</p>
<p>&lt;?output "filename.ext"?&gt;</p>
<p>&lt;?set global = 0?&gt;</p>
<p>&lt;?nextrec?&gt;</p>
<p>&lt;?include "filename.ext" ?&gt;</p>
<p>&lt;?ifchange ?&gt;</p>
<p>&lt;?if ?&gt;</p>
<p>&lt;?definegroup group-number ?&gt;</p>
<p>&lt;?ifendgroup group-number?&gt;</p>
<p>&lt;?trailing?&gt;</p>
<p>&lt;?ifnewgroup group-number?&gt;</p>
<p>&lt;?else?&gt;</p>
<p>&lt;?endif?&gt;</p>
<p>&lt;?loop?&gt;</p>
</div>

