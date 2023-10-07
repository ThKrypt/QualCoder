# Coding PDFs

PDFs can be displayed and the text on the PDF can be coded. From version 3.4.

PDFs displayed with QualCoder are not exact replicas, they are roughly displayed, due to limitations in using and understanding pdfminer and pdf structures in general. This works best with text-based PDFs, generated using text processors. The display limits are:
Some images cannot be loaded but a placeholder question mark image will be shown. Some images can have unusual colouring, or their orientation or image masking will not be reproduced. Polygons (curve objects) will be displayed but, there is not enough information to reproduce them accurately.
The screen is split into 3 panes. The Left hand side pane contains the PDF files list and codes tree. The same as other coding screens. The original fonts for text are not used (for various reasons, including it is too hard to extract the fonts and use them from within the PDFs). Instead the standard font used within QualCoder is used in the displayed PDF text boxes. There is a Font adjuster combo-box to shrink the font size, to try to avoid text overlapping. It is set at -2, and -3 may be quite good also.

The pdf plain text that is loaded when importing a PDF via Manage files must exactly match the plain text that is re-loaded when the PDF is loaded up to display the PDF here. This means that PDFs loaded before the 3.4 version will not match correctly. So it is best to only view the PDF and not code here. Selecting text boxes to code is switched off if the text lengths do not match. Similarly, if the plain text is edited in any way ad the text lengths do not match, the coding via selecting PDF text boxes is switched off. Display of the coding stripes within the  presented PDF  page may also look incorrect.

You can move through the PDF pages by clicking on the page up down arrows, or typing in a page number.

At the top of the window are several buttons. One exports an image of the PDF page. The magnifying glass button opens a window that shows the PDF elements used on the page.

Also, at the top of the window are several check boxes to show or hide PDF elements of Text, Images, and shapes of Rectangles, Lines, Curves (polygons). An extra checkbox will show all text in black which may be beneficial where there is light coloured text shown.

![pdf_screen01](https://github.com/ccbogel/QualCoder/assets/5834638/33bb51f6-a67c-456b-94ae-46e3c833eaf9)

The right hand side pane shows the plain text in the same way the text would be displayed in Code text. You can mark, unmark, memo the coded text, mark the coding as important and annotate text here.

To code, left-click and drag the mouse to select PDF text boxes. The click on a code to assign the selection to the code. Further adjustments and be made on the right-hand side plain text pane using the shift left or right arrows to extend, or the alt left and right arrows to shrink the coded text section.

Right-click for the context menu on coded area. This menu allows you to add a memo, mark important or unmark the coded segment.

### Key presses

H Show or hide the top sections of the screen.

Ctrl F jump to text search box.

Ctrl Z undo the last unmarked code.

Ctrl 1 Go to next file.

Ctrl 2 Go to latest coded file.

Ctrl 4 View and edit file memo.

Ctrl 5 Get files list from attributes.

Ctrl 8 

Ctrl 9 Show important coded segments. Toggles on and off.

Ctrl 0 Show Help page in browser.

#### In the PDF display area:

You can zoom in an out by clicking on the shown PDF and pressing + or - keys.
Press Q to quick mark selection with the recent code.
Press R to quick mark selection with a choice of recently used codes.

#### In the plain text area:

A annotate - for current selection - text edit only

Q Quick Mark with code - for current selection

I Tag important

M memo code - at clicked position

O Shortcut to cycle through overlapping codes - at clicked position

R opens a context menu for recently used codes for marking text

U Unmark at selected location

V assign 'in vivo' code to selected text

