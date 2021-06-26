Title:  Pick From

Tags:   levels-outline.6 Field Labels and Types.9 General-Purpose Fields

Timestamp: 20210609174848

Seq:    6.9.5

Level:  4 - Subsection

Body: 

This field type, when accompanied by a series of starting values, can be used to offer the user a drop-down menu allowing a choice from a set of previously used values, or the entry of a new value, which will then be added to the list. (Such a user interface widget is often referred to as a *combo box*.)

Here's an example of how you would do this in a Collection's template: 

```
Type: <pick-from: static, post>
```

In other words, enter the usual field label, followed by a colon, and then follow that with the literal 'pick-from: ', followed by the possible values, separated using commas or semicolons.
