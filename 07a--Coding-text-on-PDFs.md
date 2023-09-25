# Coding PDFs

PDFs can be displayed and the text on the PDF can be coded.

PDFs displayed with QualCoder are not exact replicas, they are roughly displayed, due to limitations in using and understanding pdfminer and pdf structures in general. The display limits are:
Some images cannot be loaded but a placeholder question mark image will be shown. Some images can have unusual colouring, or their orientation or image masking will not be reproduced. Polygons (curve objects) will be displayed but, there is not enough information to reproduce them accurately.
The screen is split into 3 panes. The Left hand side pane contains the PDF files list and codes tree. The same as other coding screens. The original fonts for text are not used (for various reasons, including it is too hard to extract the fonts and use them from within the PDFs). Instead the standard font used within QualCoder is used in the displayed PDF text boxes. There is a Font adjuster combo-box to shrink the font size, to try to avoid text overlapping. It is set at -2, and -3 may be quite good also.

At the top of the window are several check boxes to show or hide PDF elements of Text, Images, and shapes of Rectangles, Lines, Curves (polygons). An extra checkbox will show all text in black which may be beneficial where there is light coloured text shown.

![pdf_screen01](https://github.com/ccbogel/QualCoder/assets/5834638/33bb51f6-a67c-456b-94ae-46e3c833eaf9)

more here