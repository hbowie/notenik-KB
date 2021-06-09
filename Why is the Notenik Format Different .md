Title:  Why is the Notenik Format Different?

Tags:   levels-outline.2 Note Files

Timestamp: 20210608191157

Seq:    3.5

Level:  4 - Subsection

Body: 

People have been storing notes in text files long before Notenik came along.

At their most basic, such a note might consist simply of a chunk of text, with the file name serving as the note's title. 

A slightly more sophisticated approach would be to use [Markdown][md] to format a note, with a level 1 heading at the top of the file supplying a title for the note. 

The use of [MultiMarkdown metadata][meta] adds even more possibilities, allowing multiple keys and associated values to be specified at the top of a file. 

Although Notenik will read and respect all of these different sorts of text files, its own native format is a bit different from any of these. 

The Notenik format is very similar to the MultiMarkdown metadata format, but differs in that an explicit Body label is expected to indicate the start of the Note's body, rather than the body being assumed to start after the first blank line, or three hyphens, or four periods. 

So why is the Notenik format different?

The answer, in general, is that I wanted Notenik files to have a bit more flexibility than any of these other formats, without sacrificing any of their simplicity or readability. 

So whereas these other formats are primarily for documents, with at most some ability to supply metadata describing the docs, a Notenik file is an object consisting of a number of fields, with one or more of those fields containing text formatted using Markdown. 

That being said, a Notenik file is not a completely general-purpose object: it's not intended to compete with JSON or YAML, for example. For one thing, each note must have a Title field and a Body field, in addition to other fields. Also, each field generally consists of a single value, without any convention for handling arbitrary lists, or any nesting of objects. 

So there you have it: a Notenik Note sits somewhere between a Markdown doc with metadata and a full-fledged  object with any number of complex fields. Which makes it simple enough to be read and written by ordinary humans using any text editor, and yet flexible enough to help such users keep track of any number of useful, everyday objects. 

Which was exactly my intent when concocting this format. 

[md]: https://daringfireball.net/projects/markdown/syntax

[meta]: https://fletcher.github.io/MultiMarkdown-4/metadata.html

