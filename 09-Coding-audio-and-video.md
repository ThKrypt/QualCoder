# Coding audio and video

When coding video, two dialogs are displayed, shown below. One dialog has the video playing. The other dialog has the controls and a button to begin and end a coded segment. The controls window shows the codes in the bottom left pane and the .transcribed file text is shown in the bottom right pane. When coding audio, only the controls dialog is shown.

The transcription text can also be coded and annotated in this dialog window. Right-clicking on a timestamp in the transcription will give you a menu option to go to that section of the video. If a video has multiple audio tracks, you can change the audio track too. Checking the scroll checkbox allows the transcript to scroll in time with the video, based on detected timestamps, however, you need to uncheck the scroll to be able to code the transcript.

![Coding audio and video](https://qualcoder.files.wordpress.com/2021/05/code_av.png?resize=800%2C400)

_Video with coded transcript. Shown in dark mode._

## Generating Transcription using Speech-To-Text Engines
Import the a/v file into qualcoder. QualCoder will make an empty text file associated with that a/v file.
Then, while in Manage Files, double-click the a/v file to open it to view.
Underneath the transcription text box is a cogs button. Click this to open the speech to text option:

![Transcription dialog](https://user-images.githubusercontent.com/5834638/151243057-f3504e0d-ab10-4628-9495-fcdff00be422.png)

I have made it work only with a blank transcription file.

In the Speech to text dialog, select your online speech to text service of choice, add the necessary information (if required), and click on the cog at the bottom to start the speech to text conversion: 

![image](https://user-images.githubusercontent.com/55474996/151250520-d635d0c8-bb65-4a20-b6b9-e7d942c842ef.png)


## Keyboard shortcuts

* Ctrl R and Alt R are shortcuts to rewind 5 or 30 seconds
* Ctrl F will forward 30 seconds
* Ctrl S and Ctrl P will stop/start (play/pause)
* Ctrl Shift < will slow play rate down to a minimum of 0.1
* Ctrl Shift > will increase play rate up to two times.
* Ctrl Z Restores the last unmarked coding.

(These options are also available through the toolbar icons.)

When the text area has focus:

* Shortcut A. Press a to Annotate selected text

* Shortcut M. Press m to memo a code. (Must click over a coded text segment)

* Shortcut O. Press o to cycle through overlapping codes in situ. (Must click over an overlapping codes segment - denoted with an overline).

* Shortcut Q. Press q to Quick code with the most recent code. (Must have a text selection)

* Shortcut R. Press R to select Recent codes. (Must have a text selection)

## Audio Video segments

Once a segment is made using the _Start segment/Stop segment_ button this can be assigned to a code by right clicking on the relevant code and assigning the segment. 

Coding stripes for the coded segments are shown in the upper pane. Hovering the mouse over each stripe shows the code name, time segment and any memo attached to that coded segment. Right clicking on a coded segment stripe shows a menu that can be used to edit the memo, flag as an Important segment or delete the coded segment. Coded stripes are shown on various lines so that they do not overlap. 

The transcript text can also be coded and annotated in this dialog. However, when the Scroll transcript check box is checked, this cannot be performed. Playing the video when this is check will scroll the transcript using the timestamps in time with the video.

## Important coded text and segments

Important coded texts, such as exemplars for a report, can be flagged Important by using the right-click menu when on the coded text and selecting Important. Similarly, code segments can be flagged Important. At the top of the screen is a button with a star symbol. This toggles between showing all coded text and segments or Important coded text and segments.

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


## Convenience buttons underneath the files list

* Load the next file
* Load the file with the latest coding
* Open the file memo of the selected file
* Use a filter function show only those files that meet certain criteria. These can be from file attributes, or if files are associated with certain cases.

#  Categories and codes

Categories are used to organise codes. Categories are organised hierarchically in a tree structure. You can move codes into categories and move categories into larger categories. You can move categories and codes out of their current position. Codes and categories can be merged by dropping a code onto a code or a category onto a category. Categories and codes can be assigned memos. Right-click on a category or code to rename. Right click on a code to change the color.

To reduce the number of codes shown in the code tree. In the coding windows (code text, code, a/v or code image), right-click on the code tree and select Show codes like from the menu. Then enter text in the text box. This will then only show codes that contain that text. Enter nothing into the text box and press OK to show all codes again.

In the codes tree on the left, right clicking on a code opens a context menu for various options.
One option is Show coded files - this shows everywhere you have coded with the selected code. Clicking on a particular coded section will open that code in the original context for further insight.