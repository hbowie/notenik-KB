Title:  Tailor the Display

Tags:   levels-outline.3 Common Tasks.1 Display a Note

Timestamp: 20210618164350

Seq:    3.1.1

Level:  4 - Subsection

Body: 

You can alter the typeface and font size used on the Display tab by selecting the Display Appearance item under the Format menu, or by clicking on the Display Fonts button on the toolbar. You may then pick a typeface and font from the displayed dropdown menus or, if you'd like, enter the CSS you'd like to be used directly, bypassing the limits of these menus. The default font list only includes a relatively short list of common fonts; by checking the box to use the long list, showing all fonts, the user may select any font family available on your Mac. 

The Collection Preferences contain a couple of options for changing the way a Note is formatted on the Display tab.

+ Include explicit Body field label on the Display tab? - This is checked by default, but you can uncheck this option if you'd prefer the body to just show up without any header label. 

+ Display Note Titles as Level 1 Headings? - The default is to display note titles as paragraphs with strong emphasis, but check this box if you'd prefer them to be displayed within `h1` tags.

The layout and appearance of the Display tab for a particular Collection can be further customized by the addition of either of the following special files to the folder containing a Collection's notes. 

+ `display.css` -- Enter whatever custom CSS you would like to alter the appearance of a Note on the Display tab. 

+ `display.html` -- Enter a Merge Template (following the rules for [[Merge Templates]]) to alter the layout of the Display tab in any way you would like. If this file is present, then it should contain the CSS to be used (rather than putting it into the separate file mentioned above). This file should start with a `<?nextrec?>` command and end with a `<?loop?>` command, and should not include an `<?output?>` command. 

Note that you may use the `Generate Sample Display Template` command beneath the `Collection` menu to have Notenik generate samples of both of these files. You may then delete one or the other, and modify the remaining file, to achieve your desired effects.
