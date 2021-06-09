Title:  Note File Format

Tags:   levels-outline.3 Note Files

Timestamp: 20210608185058

Seq:    3.1

Level:  4 - Subsection

Body: 

The contents of each Notenik Note file are formatted in a way that is easy to read and write, for both humans and computers, but is somewhat special, and unique to Notenik. 

Here are the general formattng rules:

+ A Note consists of a series of Fields. 

+ Each Field consists of an identifying label, followed by a value. 

+ The label can be spelled out in typically human fashion, with capitalization and spacing. 

+ The label must be immediately followed by a colon, and the colon must be followed by one or more spaces. 

+ Most values are specified on the same line as the label, but multi-line values (for types such as longtext, teaser, code, body, etc.) can be specified on following lines. 

+ One blank line should separate each Field (in other words, each label-value combination) from the beginning of the next Field. 

+ The Title Field must come first. 

+ The Body Field must be last. 

+ Once the Body label is encountered, everything following will be interpreted as part of the Body's value.
