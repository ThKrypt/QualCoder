# Coding Text

Select Code text from the Coding menu. This is the central dialog for assigning codes to text. Once text segments are coded, hovering the mouse over the coding shows the code name as a tooltip. Clicking on the coded segment also shows the code name. 

![Code text screen](https://qualcoder.files.wordpress.com/2021/05/code_text-1.png?resize=700%2C500)

Select a file for coding from the selection list on the left. The file selection list contains buttons that allow you to move to the next file, to move to the most recently coded file and to go to a bookmarked position in a file. There is also a button to view the file memo.

Create a new code by right-clicking in the left hand window. Codes can  be assigned a colour by right-clicking on the code and selecting the change code colour option. Other options from the right-click menu include adding a memo to the code, deleting the code, renaming, adding a new code, and adding a new category.

The easiest way to code text, is to select some text, then left-click with the mouse on a code. A second way is to select a code, then select some text. Right-click and mark the text to assign it to the selected code. Hover the mouse pointer over coded text to see a tooltip of the code. Coded text can be uncoded by clicking on the text segment and pressing the Unmark button.

Coded text segments can be memoed - through the right-click menu, by pressing 'm' or by clicking on the pencil and red notepad icon. Text under a code with a memo is italicised.

Important coded texts, such as exemplars for a report, can be flagged Important by using the right-click menu when on the coded text and selecting Important. The button wit hthe start underneath the codes tree toggles between showing all coded text and coded text flagged as important.

## Overlapping codes

Overlapping codes can be difficult to view clearly. Overlaps have an overline above the text to show overlapping sections and are italicised (coded text with a code memo is also italicised). Mouse hover will show coded text, including overlaps. Clicking in an overlap shows a selection box at the top of the screen where you can select to view one or the other highlighted coded text.
You can also press 'O' after clicking on an overlapping section to cycle through the codes there.

## Annotations
Add an annotation (like a memo for a text segment) to a text selection. The text will become bold to mark the position of the annotation. To re-open an annotation, select some of the bolded-text and right-click to get the Annotate option. Alternatively, click the notepad and pencil icon on the left, or press the 'a' key.

![annotation](https://qualcoder.files.wordpress.com/2019/01/annotation.png?w=429&h=240)

## Auto-code

The top right of the dialog has icons for auto-coding text. The top right section has buttons for auto-coding text. 

You can:
* auto-code exact text
* auto-code sentences based on a text fragment in the current file
* auto-code sentences based on a text fragment for all files
* auto-code the current file using start and end text marks. You can use ‘\n’ for a line ending character. The start mark text is included in the coded section.
* Undo previous auto-coding

Automatic coding is case sensitive. You must also define the end of a sentence, there is a default setting with a period and space. \n can be used also to denote a line ending character.
For auto-coding exact text matches, multiple sections of text can be assigned by auto code using the pipe ‘|’ symbol. For example, politics|politicians can be assigned to the same code at the same time (for exact auto code text matches only). There is an undo option to undo recently performed auto-coding. Although if the project is closed and reopened, the undo option will be lost.

## Maximise screen area
To hide the top control panel, click in the text area and press the 'h' key. To show the top panel, press 'h' again.

## Convenience methods for loading text files in the files list pane.

Some projects may have many text files and the view file dialog may present too many files to open. Right-click on the files in the file tree button to go to the next file, go to the bookmarked file or go to the file with the latest codings: 

* The next file alphabetically, 

* Select the file which was most recently coded, 
* Go to a bookmarked location in a file. To create a bookmark, right click in some text when coding and select the bookmark option. The bookmark works for only one project at a time, so if you opened a different project, the bookmark would be incorrect or might not work at all.

### Convenience buttons underneath the files list

* Load the next file
* Load the file with the latest coding
* Go to the currently bookmarked file
* Open the file memo of the selected file
* Use a filter function show only those files that meet certain criteria. These can be from file attributes, or if files are associated with certain cases. (Image below)

![Code text and selecting parameters to show only the matching files](https://qualcoder.files.wordpress.com/2021/05/code_text_parameters.png?resize=700%2C500)


## Large text files
Large text files slow QualCoder. When opening a large text file (greater than 50,000 characters), right click on the file. A menu option allows you to get the first approximately 50,000 characters, subsequent clicks will open the next approximately 50,000 and so on. Approximately, because QualCoder looks for a line-ending (such as a paragraph or sentence ending) to more nicely section the start and end of text chunks.

## Modifying code positions

When in the text area, click on a code with the mouse (Note the code must not be overlapping with another code at that position). Press the following key combinations to extend or shrink the coded text segment.

* Shift + left arrow            Extends coded text to the left
* Shift + right arrow          Extends coded text to the right
* Alt + left arrow               Shrinks coded text from the right hand side towards the left
* Alt + right arrow            Shrinks coded text from the left hand side towards the right

You can also right-click on a code and select change start position or change end position by  a number of characters.

## Other shortcut keys for text coding

* Shortcut A. Press a to Annotate selected text

* Shortcut B. Press b to bookmark the current location in the current text file.

* Shortcut R. Press r to select Recent codes. (Must have a text selection)

* Shortcut Q. Press q to Quick code with the most recent code. (Must have a text selection)

* Shortcut M. Press m to memo a code. (Must click over a coded text segment)

* Shortcut O. Press o to cycle through overlapping codes in situ. (Must click over an overlapping codes segment - denoted with an overline).

* Shortcut H. Press h will hide and unhide the top section of controls on the screen. This provides a bigger area to view the text and to code.

* Shortcut i. Press i when on a coded section to mark that code as important. Useful for identifying exemplars. Important marks can be removed by right-click and selecting Remove important mark. Important marked codes are bolded.

* Ctrl E. Enter and exit text edit mode.

## Search text

The coding text dialog contains a search for text function at the top middle, with tick boxes for searching case sensitive and for searching through all text files. When in the text area, selecting some text and pressing the shortcut key ‘s’ will fill the search text box and focus on the ‘next’ arrow button for quickly looking through the document for the selected text. The search requires a minimum of 3 characters. The Case sensitive check box will limit to case sensitive searching. The All files check box will continue the search through other text files.

The search uses Regex functions. 

* A dot ‘.’ is used as a wild card, e.g. ‘.ears’ will match ‘bears’ and ‘years’. 
* A ‘?’ after a character will match one or none times that character, e.g. ‘bears?’ will match ‘bear’ and ‘bears’ 
* A ‘*’ after a character will match zero or more times. 
* ‘\. will match the dot symbol, ‘\?’ will match the question mark. ‘\n’ will match the line ending symbol. This Regex cheatsheet might assist: www.rexegg.com/regex-quickstart.html
* \b word boundary, ‘\bbound\b’ will search for the full word ‘bound’, but not ‘boundary’

## Moving through the text for one selected code

Underneath the codes tree are the buttons: forward, back and a grid icon button (to exit the function).

Select a code and then click on the forward and back arrows. These now traverse through the text document showing the selected coded text. All other coded text is hidden. To restore and show all the codes, click on the now coloured grid button.

** Show only important coded text

Under the codes tree is a button with a star symbol. This button toggles between showing all coded text and the coded text flagged as Important.

# Right-hand hidden pane

The right hand side of the coding text pane has another pane tucked away. To open click and drag from the right-hand side of the window. This pane contains three options useful when coding. One option is when clicking on a code, the code name, code rule (memo) and random code examples are displayed. The J button displays an editable current journal, determined by the most recent date. The P button displays the editable project memo.

# Editing text (Ctrl E)

Text can be edited even after the text is coded or annotated or assigned (fully or partially) to a case. Click on the text area and press Ctrl E to enter and exit text mode.
This feature is in releases 2.7 and up: Sections of the text file or audio/video transcribed file will have sections of text underlined in green (case assigned), yellow (annotation) or red (coded) by ALL coders. 

When entering the edit mode, the entire file is loaded for editing. Other functions such as the codes tree and file list are deactivated.

You can select text that is not underlined and copy/replace without problems. You can click on a position (without selecting text) to then type, delete, or paste text. This can occur in underlined (coded, annotated, case-assigned) or not underlined (not coded/annotated/case-assigned) text locations. You will see the underlines shift as text is added or removed.

There are some limitations: It is best to avoid selecting sections of text to delete (or to type or paste over). This is particularly an issue if any of those sections have been underlined (coded, annotated, case-assigned). It may also be an The reason is that positions of the underlying codes/annotations/case-assigned may not correctly match as intended. If you have made a change that you think has affected these coded/annotated/case-assigned positions badly, exit the text editing window by pressing the Cancel button.

**Important note: The edits occur within the database. The original text file is NOT changed.** 


#  Categories and codes

Categories are used to organise codes. Categories are organised hierarchically in a tree structure. You can move codes into categories and move categories into larger categories. You can move categories and codes out of their current position. Codes and categories can be merged by dropping a code onto a code or a category onto a category. Categories and codes can be assigned memos. Right-click on a category or code to rename. Right click on a code to change the color.

To reduce the number of codes shown in the code tree. In the coding windows (code text, code, a/v or code image), right-click on the code tree and select Show codes like from the menu. Then enter text in the text box. This will then only show codes that contain that text. Enter nothing into the text box and press OK to show all codes again.

In the codes tree on the left, right clicking on a code opens a context menu for various options.
One option is Show coded files - this shows everywhere you have coded with the selected code. Clicking on a particular coded section will open that code in the original context for further insight.

[YouTube Video QualCoder 2.7 - Coding Text](https://www.youtube.com/watch?v=-8LnXfcM0cw&t=0s)



