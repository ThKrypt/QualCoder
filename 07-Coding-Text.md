# Coding Text

Select Code text from the Coding menu. This is the central dialog for assigning codes to text. Once text segments are coded, hovering the mouse over the coding shows the code name as a tooltip. Clicking on the coded segment also shows the code name. 

![Coding text dialog](https://qualcoder.files.wordpress.com/2020/12/code_text.png)

Select a file for coding from the selection list on the left. The file selection list contains buttons that allow you to move to the next file, to move to the most recently coded file and to go to a bookmarked position in a file. There is also a button to view the file memo.

Create a new code by right-clicking in the left hand window. Codes can  be assigned a colour by right-clicking on the code and selecting the change code colour option. Other options from the right-click menu include adding a memo to the code, deleting the code, renaming, adding a new code, and adding a new category.

The easiest way to code text, is to select some text, then left-click with the mouse on a code. A second way is to select a code, then select some text. Right-click and mark the text to assign it to the selected code. Hover the mouse pointer over coded text to see a tooltip of the code. Coded text can be uncoded by clicking on the text segment and pressing the Unmark button.

Coded text segments can be memoed - through the right-click menu, by pressing 'm' or by clicking on the pencil and red notepad icon.

The tooltip is shown in the below image of overlapping codes.

Overlapping codes can be difficult to view clearly. Overlaps have an overline above the text to show overlapping sections. Mouse hover will show coded text, including overlaps. Clicking in an overlap shows a selection box at the top of the screen where you can select to view one or the other highlighted coded text.

![overlapping codes](https://qualcoder.files.wordpress.com/2020/12/overlapping.png)


**Annotations**
Add an annotation (like a memo for a text segment) to a text selection. The text will become bold to mark the position of the annotation. To re-open an annotation, select some of the bolded-text and right-click to get the Annotate option. Alternatively, click the notepad and pencil icon on the left, or press the 'a' key.

![annotation](https://qualcoder.files.wordpress.com/2019/01/annotation.png?w=429&h=240)

**Auto-code**

The top right of the dialog has icons for auto-coding text. You can auto-code exact text, auto-code sentences based on a text fragment in the current file, and auto-code sentences based on a text fragment for all files. You must also define the end of a sentence, there is a default setting with a period and space. For auto-coding exact text matches, multiple sections of text can be assigned by auto code using the pipe ‘|’ symbol. For example, politics|politicians can be assigned to the same code at the same time (for exact auto code text matches only). There is an undo option to undo recently performed auto-coding. Although if the project is closed and reopened, the undo option will be lost.

## Convenience methods for loading text files

Some projects may have many text files and the view file dialog may present too many files to open. Right-click on the View File button to select options such as: 

* The next file alphabetically, 

* Select the file which was most recently coded, 
* Go to a bookmarked location in a file. To create a bookmark, right click in some text when coding and select the bookmark option. The bookmark works for only one project at a time, so if you opened a different project, the bookmark would be incorrect or might not work at all.

## Modifying code positions

When in the text area, click on a code with the mouse (Note the code must not be overlapping with another code at that position). Press the following key combinations to extend or shrink the coded text segment.

* Shift + left arrow            Extends coded text to the left
* Shift + right arrow          Extends coded text to the right
* Alt + left arrow               Shrinks coded text from the right hand side towards the left
* Alt + right arrow            Shrinks coded text from the left hand side towards the right

You can also right-click on a code and select change start position or change end position by  a number of characters.

**Other shortcut keys for text coding:**

* Shortcut A. Press a to Annotate selected text

* Shortcut B. Press b to bookmark the current location in the current text file.

* Shortcut R. Press r to select Recent codes. (Must have a text selection)

* Shortcut Q. Press q to Quick code with the most recent code. (Must have a text selection)

* Shortcut M. Press m to memo a code. (Must click over a coded text segment)

* Shortcut O. Press o to cycle through overlapping codes in situ. (Must click over an overlapping codes segment - denoted with an overline).

* Shortcut H. Press h will hide and unhide the top section of controls on the screen. This provides a bigger area to view the text and to code.

**Search text**

The coding text dialog contains a search for text function at the top middle, with tick boxes for searching case sensitive and for searching through all text files. When in the text area, selecting some text and pressing the shortcut key ‘s’ will fill the search text box and focus on the ‘next’ arrow button for quickly looking through the document for the selected text. The search requires a minimum of 3 characters. The Case sensitive check box will limit to case sensitive searching. The All files check box will continue the search through other text files.

The search uses Regex functions. 

* A dot ‘.’ is used as a wild card, e.g. ‘.ears’ will match ‘bears’ and ‘years’. 
* A ‘?’ after a character will match one or none times that character, e.g. ‘bears?’ will match ‘bear’ and ‘bears’ 
* A ‘*’ after a character will match zero or more times. 
* ‘\. will match the dot symbol, ‘\?’ will match the question mark. ‘\n’ will match the line ending symbol. This Regex cheatsheet might assist: www.rexegg.com/regex-quickstart.html
* \b word boundary, ‘\bbound\b’ will search for the full word ‘bound’, but not ‘boundary’


#  Categories and codes

Categories are used to organise codes. Categories are organised hierarchically in a tree structure. You can move codes into categories and move categories into larger categories. You can move categories and codes out of their current position. Codes and categories can be merged by dropping a code onto a code or a category onto a category. Categories and codes can be assigned memos. Right-click on a category or code to rename. Right click on a code to change the color.

To reduce the number of codes shown in the code tree. In the coding windows (code text, code, a/v or code image), right-click on the code tree and select Show codes like from the menu. Then enter text in the text box. This will then only show codes that contain that text. Enter nothing into the text box and press OK to show all codes again.

In the codes tree on the left, right clicking on a code opens a context menu for various options.
One option is Show coded files - this shows everywhere you have coded with the selected code. Clicking on a particular coded section will open that code in the original context for further insight.

