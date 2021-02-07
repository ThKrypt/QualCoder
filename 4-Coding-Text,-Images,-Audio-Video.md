#  Categories and codes

Categories are used to organise codes. Categories are organised hierarchically in a tree structure. You can move codes into categories and move categories into larger categories. You can move categories and codes out of their current position. Codes and categories can be merged by dropping a code onto a code or a category onto a category. Categories and codes can be assigned memos. Right-click on a category or code to rename. Right click on a code to change the color.

To reduce the number of codes shown in the code tree. In the coding windows (code text, code, a/v or code image), right-click on the code tree and select Show codes like from the menu. Then enter text in the text box. This will then only show codes that contain that text. Enter nothing into the text box and press OK to show all codes again.

In the codes tree on the left, right clicking on a code opens a context menu for various options.
One option is Show coded files - this shows everywhere you have coded with the selected code. Clicking on a particular coded section will open that code in the original context for further insight.

# Coding Text

Select Code text from the Coding menu. This is the central dialog for assigning codes to text. Once text segments are coded, hovering the mouse over the coding shows the code name as a tooltip. Clicking on the coded segment also shows the code name. 

![Coding text dialog](https://qualcoder.files.wordpress.com/2020/12/code_text.png)

Select a file for coding from the selection list on the left. The file selection list contains buttons that allow you to move to the next file, to move to the most recently coded file and to go to a bookmarked position in a file. There is also a button to view the file memo.

Create a new code by right-clicking in the left hand window. Codes can  be assigned a colour by right-clicking on the code and selecting the change code colour option. Other options from the right-click menu include adding a memo to the code, deleting the code, renaming, adding a new code, and adding a new category.

The easiest way to code text, is to select some text, then left-click with the mouse on a code. A second way is to select a code, then select some text. Right-click and mark the text to assign it to the selected code. Hover the mouse pointer over coded text to see a tooltip of the code. Coded text can be uncoded by clicking on the text segment and pressing the Unmark button.

Coded text segments can be memoed - through the right-click menu or by clicking on the pencil and red notepad icon.

The tooltip is shown in the below image of overlapping codes.

Overlapping codes can be difficult to view clearly. Overlaps have an overline above the text to show overlapping sections. Mouse hover will show coded text, including overlaps. Clicking in an overlap shows a selection box at the top of the screen where you can select to view one or the other highlighted coded text.

![overlapping codes](https://qualcoder.files.wordpress.com/2020/12/overlapping.png)


**Annotations**
Add an annotation (like a memo for a text segment) to a text selection. The text will become bold to mark the position of the annotation. To re-open an annotation, select some of the bolded-text and right-click to get the Annotate option. Alternatively, click the notepad and pencil icon on the left.

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

* Shortcut A to Annotate selected text

* Shortcut B to bookmark the current location in the current text file.

* Shortcut R to select Recent codes. (Must have a text selection)

* Shortcut Q to Quick code with the most recent code. (Must have a text selection)

* Shortcut M to memo a code. (Must click over a coded text segment)

* Shortcut O to cycle through overlapping codes in situ. (Must click over an overlapping codes segment - denoted with an overline).

**Search text**

The coding text dialog contains a search for text function at the top middle, with tick boxes for searching case sensitive and for searching through all text files. When in the text area, selecting some text and pressing the shortcut key ‘s’ will fill the search text box and focus on the ‘next’ arrow button for quickly looking through the document for the selected text. The search requires a minimum of 3 characters. The Case sensitive check box will limit to case sensitive searching. The All files check box will continue the search through other text files.

The search uses Regex functions. 

* A dot ‘.’ is used as a wild card, e.g. ‘.ears’ will match ‘bears’ and ‘years’. 
* A ‘?’ after a character will match one or none times that character, e.g. ‘bears?’ will match ‘bear’ and ‘bears’ 
* A ‘*’ after a character will match zero or more times. 
* ‘\. will match the dot symbol, ‘\?’ will match the question mark. ‘\n’ will match the line ending symbol. This Regex cheatsheet might assist: www.rexegg.com/regex-quickstart.html
* \b word boundary, ‘\bbound\b’ will search for the full word ‘bound’, but not ‘boundary’

#  Coding images

Images can be coded in a similar way to text coding. Select a code. Left-click and drag to highlight the area you want to assign to the code. Right-click will open a menu where you can remove the coding or add a memo. At the bottom of the screen there is a slider control to re-size the image. Coded rectangles are coloured to match the code colour. 

The top right of the dialog shows some details of a clicked on coded area - by showing the code name pixel positions and percentage area of the entire image. Hovering the mouse over this space will show any memo for the coded area.

![coding image](https://qualcoder.files.wordpress.com/2020/12/image-coding.png)

# Coding audio and video

When coding video, two dialogs are displayed, shown below. One dialog has the video playing. The other dialog has the controls and a button to begin and end a coded segment. The controls window shows the codes in the bottom left pane and the .transcribed file text is shown in the bottom right pane. When coding audio, only the controls dialog is shown.

The transcription text can also be coded and annotated in this dialog window. Right-clicking on a timestamp in the transcription will give you a menu option to go to that section of the video. If a video has multiple audio tracks, you can change the audio track too. Checking the scroll checkbox allows the transcript to scroll in time with the video, based on detected timestamps, however, you need to uncheck the scroll to be able to code the transcript.

![Coding audio and video dialogs](https://qualcoder.files.wordpress.com/2020/12/code_video.png)

## Keyboard shortcuts

* Ctrl R and Alt R are shortcuts to rewind 5 or 30 seconds
* Ctrl F will forward 30 seconds
* Ctrl S and Ctrl P will stop/start (play/pause)
* Ctrl Shift < will slow play rate down to a minimum of 0.1
* Ctrl Shift > will increase play rate up to two times.

(These options are also available through the toolbar icons.)

When the text area has focus:

* Shortcut A to Annotate selected text

* Shortcut M to memo a code. (Must click over a coded text segment)

* Shortcut O to cycle through overlapping codes in situ. (Must click over an overlapping codes segment - denoted with an overline).

* Shortcut Q to Quick code with the most recent code. (Must have a text selection)

* Shortcut R to select Recent codes. (Must have a text selection)

## Audio Video segments

Once a segment is made using the _Start segment/Stop segment_ button this can be assigned to a code by right clicking on the relevant code and assigning the segment. 

Coding stripes for the coded segments are shown in the upper pane. Hovering the mouse over each stripe shows the code name, time segment and any memo attached to that coded segment. Right clicking on a coded segment stripe shows a menu that can be used to edit he memo or delete the coded segment. Coded stripes are shown on various lines so that they do not overlap. 

The transcript text can also be coded and annotated in this dialog. However, when the Scroll transcript check box is checked, this cannot be performed. Playing the video when this is check will scroll the transcript using the timestamps in time with the video.

**Linking text to coded segments**

There are two ways to link text and coded segments. One way is to select text (it can be coded or preferably uncoded) then assign it to a segment. First select the text and right-click Prepare text link to segment. Then right-click on the receiving segment, choose Link text to segment, to assign the text.

A second way is to select a segment and link it to a text selection via a similar process.


## Modifying code positions in the text area

When in the text area, click on a code with the mouse (Note the code must not be overlapping with another code at that position). Press the following key combinations to extend or shrink the coded text segment.

* Shift + left arrow            Extends coded text to the left
* Shift + right arrow          Extends coded text to the right
* Alt + left arrow               Shrinks coded text from the right hand side towards the left
* Alt + right arrow            Shrinks coded text from the left hand side towards the right

You can also right-click on a code and select change start position or change end position by  a number of characters.

## The video window

On the video window you can right-click and have options to change the window size, in pixels. You can also export a screenshot. The screenshot will be save as Frame_yyyymmdd_hh_mm_ss.jpg in the directory listed in the Settings.




