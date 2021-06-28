Title:  Assembling an Outline

Tags:   fields.index, fields.level, fields.seq

Timestamp: 20210628023650

Seq:    10.1

Level:  3 - Section

Index:  streamlined reading; 

Body: 

In many cases, the Notes within a Collection will bear little relationshp to each other. 

In some cases, the [[Tags]] field may be used to group Notes together by topic. 

In other cases, Notes within a Collection may be organized by [[Date]].

But in addition to these other organizational paradigms, Notenik has several related capabilites that allow the Notes within a Collection to be assembled into an [outline](https://en.wikipedia.org/wiki/Outline_(list)). 

1. The first step is to add a [[Seq]] field to your Collection. This field can then be used to place your Notes into a meaningful sequence. 

2. Next, add a [[Level]] field to the Collection. Make [[use of a text editor]] to modify [[the Collection template file]] to specify how many levels your outline will have, with the top level being 1. You can assign some meaningful bit of text to each number, to make it easier to keep things straight as you are adding Notes to your Collection. Level 1 can be used to represent the top level for the entire Collection.  

3. Then make a couple of adjustments to your Collection Preferences. Uncheck the box that says "Include explicit Body field label on the Display tab," and check the box that says "Format Display for Streamlined Reading."

4. Now start populating your Collection. Set the Sort parm for the Collection to `Seq + Title`.  Your very first Note should probably represent the top level for the entire Collection, and be assigned a Level of 1, while setting the Seq to `0`, or simply leaving the Seq field blank. 

5. Now build out your outline, using the Level to indicate the depth of each Note within the outline, and using Seq plus Level to indicate the relationships between parents and children. 

6. Note that, on the List tab, your Note titles will be indented to indicate the Level of each Note. 

7. For an outline structure, it's usually handy to assign Seq values so that the numbers assigned indicate the outline structure. For example, a Note with a Seq value of 3.2.4 would be the fourth child of the Note with a Seq value of 3.2.

8. If you need to insert a Note into the sequence you are building, you can use the `Note -> Increment` menu item to increment the Seq value of the selected Note, as well as all following Notes, in order to preserve the existing order and make room for a new Note at the original Seq value of the incremented Note. 

9. In order to have the Seq value incremented automatically for a new Note, first select the preceding Note before adding the new one. 

10. As you continue building out your outline, you may wish to make use of a couple of helpful menu items beneath the `Collection` menu. 

	+ `Collection -> Level -> Renumber Seq based on Level` will renumber your entire Collection, preserving the current order, but regenerating Seq values so that each segment of each Seq value is numbered consecutively, without any gaps, and with the number of segments reflecting each Note's level. 

	+ `Collection -> Level -> Replace Tags based on Seq and Level` will generate Tags with a top level of `levels-outline`, and with sub-tags mirroring the structure of your outline. The advantage of navigating your Collection this way is that you will have disclosure triangles, allowing you to drill down to a particular point in the outline, while hiding other branches not currently of interest. 

Note that, if you have followed all the instructions above, including modifying your Collection preferences, your Display tab will now look a little different. 

+ Fields other than Seq, Title and Body will not be shown. 
+ The Seq Value will be shown at the beginning of the Title line. 
+ For Notes with a level greater than 1, a link to the implied parent Note will be shown at the top of the display. 
+ For Notes with two or more children, a "Contents" section will appear below the body of the selected Note, with links to each of that Note's children.
+ At the very bottom of the display, for every Note other than the last, you will see a link to the next Note in the sequence. 

You will now find that, using the links described above, you can navigate through your entire Collection entirely within the Display tab. 

If you'd like, you can use the `View -> Show/Hide List` menu item to completely hide the List and Tags tabs. 

The overall intent of all this is to provide a "streamlined reading" experience for your Collection, focusing on the outline structure and the content, much as you would when reading a book.

And one last tip for a project like this. If you add an [[Index]] field, and then use that to provide index terms for your pages, then you can use the `Collection -> Generate Index` menu item to generate an index for your Collection (as you might find at the end of a book). The index will be formatted using Markdown, and copied to the system clipboard. Simply create an index Note in your Collection, and use a normal paste command to place your index into the body of your index Note.
