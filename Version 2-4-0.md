Title:  Version 2.4.0

Tags:   levels-outline.11 Version History.42 Version 240

Timestamp: 20210627222923

Seq:    11.43

Level:  3 - Section

Body: 

Released on 13 Dec 2019
 
##### Added Startup Check

Added a logic check to see if the app completed a successful launch the last time it was run. If not, then the application resets the user preferences to avoid a recurring crash. 

 
##### Added Note-to-Note Linking

Wiki-style links between Notes within a Collection are now supported. Several related pieces of functionality work together to enable this capability. 

* The Collection Preferences pane now includes a checkbox for "Double Bracket Parsing for Inter-Note Links". Turning this option on for a particular Collection allows the user to begin adding links between Notes. 

* Once this option is enabled, the body of a Note may include a link to another Note by enclosing the title of that other Note within double square brackets. 

* A new Variable Modifier of 'W' available in Merge Templates allows these inter-note pointers to be converted to usable links when generating HTML.