Title:  Filter Module Parameters

Tags:   levels-outline.8 Script Files.2 Scripting Modules

Timestamp: 20210617211436

Seq:    9.2.2

Level:  4 - Subsection

Body: 

A filter command may have an action of 'clear', 'add' or 'set'.

#### Clear

Clears any filter parameters that might have previously been set, so that new ones can be added. A clear action must be followed by a set action in order to actually remove any previously specified filtering rules. 

#### Add

Adds a new filter rule. The object would name the field to be compared as part of the filter. The value field would specify a value to which the object will be compared. And the modifier field specifies the nature of the comparison. 

The following modifiers are valid (with all of the different forms on a line producing identical results).

* "=", "==", "eq" or "equals"

* ">", "gt" or "greater than"

* ">=", "!<", "ge" or "greater than or equal to"

* "<", "lt" or "less than"

* "<=", "!>", "le" or "less than or equal to"

* "<>", "!=", "ne" or "not equal to"

* "()", "[]", "co" or "contains"

* "!()", "![]", "nc" or "does not contain"

* "(<)", "[<]", "st" or "starts with"

* "!(<)", "![<]", "ns" or "does not start with"

* "(>)", "[>]", "fi" or "ends with"

* "!(>)", "![>]", "nf" or "does not end with"

#### Set

An action of set causes the previously added filtering rules, specified since the last clear action, to be applied.
