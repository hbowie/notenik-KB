Title:  Email Apostrophes

Tags:   levels-outline.7 Merge Templates.3 Variable Modifiers

Timestamp: 20210616194522

Seq:    7.3.1

Level:  4 - Subsection

Body: 

Placing a single apostrophe (`'`) as part of the variable modifiers string will cause any HTML entities representing an apostrophe to be converted back to a normal ASCII/UTF apostrophe character: '. This can be useful for generating HTML to use as e-mail content, since e-mail parsers seem to sometimes drop the HTML entities commonly used for apostrophes.

