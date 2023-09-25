# Coding PDFs

PDFs can be displayed and the text on the PDF can be coded. From version 3.4.

PDFs displayed with QualCoder are not exact replicas, they are roughly displayed, due to limitations in using and understanding pdfminer and pdf structures in general. The display limits are:
Some images cannot be loaded but a placeholder question mark image will be shown. Some images can have unusual colouring, or their orientation or image masking will not be reproduced. Polygons (curve objects) will be displayed but, there is not enough information to reproduce them accurately.
The screen is split into 3 panes. The Left hand side pane contains the PDF files list and codes tree. The same as other coding screens. The original fonts for text are not used (for various reasons, including it is too hard to extract the fonts and use them from within the PDFs). Instead the standard font used within QualCoder is used in the displayed PDF text boxes. There is a Font adjuster combo-box to shrink the font size, to try to avoid text overlapping. It is set at -2, and -3 may be quite good also.

The pdf plain text that is loaded when importing a PDF via Manage files must exactly match the plain text that is re-loaded when the PDF is loaded up to display the PDF here.

You can move through the PDF pages by clicking on the page up down arrows, or typing in a page number.

At the top of the window are several buttons. One exports an image of the PDF page. The magnifying glass button opens a window that shows the PDF elements used on the page.

Also, at the top of the window are several check boxes to show or hide PDF elements of Text, Images, and shapes of Rectangles, Lines, Curves (polygons). An extra checkbox will show all text in black which may be beneficial where there is light coloured text shown.

![pdf_screen01](https://github.com/ccbogel/QualCoder/assets/5834638/33bb51f6-a67c-456b-94ae-46e3c833eaf9)

The right hand side pane shows the plain text in the same way the text would be displayed in Code text. You can mark, unmark, memo the coded text, mark the coding as important and annotate text here.

In the PDF window itself. You can zoom in an out by clicking on the shown PDF and pressing + or - keys.

To code, left-click and drag the mouse to select PDF text boxes. The click on a code to assign the selection to the code. Further adjustments and be made on the right-hand side plain text pane using the shift left or right arrows to extend, or the alt left and right arrows to shrink the coded text section.

