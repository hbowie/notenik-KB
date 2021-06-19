Title:  Rules for Reading

Tags:   levels-outline.5 Existing Text Files

Timestamp: 20210608235050

Seq:    4.7.1

Level:  4 - Subsection

Body: 

With that being said, here are some rules that Notenik will try to apply to interpret existing text files in the best possible manner. (Many or even most of these rules involve recognition of the start of the note's body, even though the note lacks the explicit `Body:` field label found in the standard Notenik format.)

1. Notenik will respect a template file that it finds, but it does not insist on the presence of a template file. 

2. Notenik will place a file named ``- INFO.nnk` in any folder that it opens successfully. Notenik uses this file to track some basic info about the Collection. Notenik also uses the presence of this file to indicate that the folder contains a Notenik Collection. 

3. Notenik will generally respect whatever metadata tags are found at the top of the file, unless you have specified otherwise. In this respect, Notenik generally follows the same conventions as the [MultiMarkdown Metadata](https://fletcher.github.io/MultiMarkdown-4/metadata.html) specification. 

4. In accordance with this same spec, Notenik will respect a line of three dashes before and after the metadata, to indicate the start and end of the metadata block. The line after the metadata can also be one to four periods. 

5. Notenik normally expects to see blank lines between metadata fields, for improved readability. However, if the first line contains a Title field, and is immediately followed by another metadata field, without an intervening blank line, then Notenik will assume that the first blank line encountered should end the metadata block and start the body of the note. 

6. If a file does not begin with any metadata, but starts with a normal [Markdown level 1 heading](https://daringfireball.net/projects/markdown/syntax#header), then Notenik will use the contents of that heading as the title of the note. 

7. If a file does not start with either metadata or a Markdown level 1 heading, then Notenik will use the file name (dropping the file extension) as the title of the note, and use the entire contents of the file as the body. 

8. If a file does not start with metadata, but does start with a Markdown level 1 heading, then the second line of the file may use a '#', immediately followed by text (without any intervening spaces) to indicate that the text should be treated as tags for the note. I'm not quite sure where this convention originated, or how many people use it, but there it is.
