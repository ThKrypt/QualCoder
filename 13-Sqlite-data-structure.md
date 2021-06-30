The current v3 data structure is described to assist with developing sql queries. Tables are listed alphabetically.

# Table: annotation

**anid** integer  A unique auto-number

**fid** integer Links to the source.id. Annotations are only for text files.

**pos0** integer  The starting character position in the text file.

**pos1** integer  The ending character position in the text file.

**memo** text  Contains the annotation text.

**owner** text  The coder who created the entry.

**date** text  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

# Table: attribute

**attrid** integer  A unique auto-number.

**name** text The name of the attribute. This will match the name in attribute_type.

**attr_type** text  This is either 'case' or 'file'

**value** text This store the attribute value as text, even if it is meant to be a numeric value. You may need to cast(value as real)

**id** integer This field represents a source id or a case id.

**owner** text  The coder who created the entry.

**date** text  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

# Table: attribute_type

**name** text  The unique name of the attribute.

**owner** text  The coder who created the entry.

**date** text  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

**memo** text  Contains a memo about the attribute type.

**caseOrFile** text  This is either 'case' or 'file' 

**valuetype** text  This is either 'character' or 'numeric'

# Table: case_text

**id** integer Unique autonumber.

**caseid** integer  Links to the cases.caseid.

**fid** integer links to the source.id. These are only for text files.

**pos0** integer  The starting character position in the text file. Null if not a text file.

**pos1** integer  The ending character position in the text file.  Null if not a text file.

**memo** text  Contains the memo text.

**owner** text  The coder who created the entry.

**date** text  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

# Table: cases

**caseid** integer  A unique auto-number.

**name** text   The name of the case.

**memo** text  Contains the memo text.

**owner** text  The coder who created the entry.

**date** text  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

# Table: code_av

**avid** integer  A unique auto-number.

**id** integer  Links to the source.id to identify the source A/V file.

**pos0** integer  The starting milliseconds position in the A/V file.

**pos1** integer  The ending milliseconds position in the A/V file.

**cid** integer  The code_name id to identify the code.

**memo** text  Contains the memo text.

**owner** text  The coder who created the entry.

**date** text  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

**important** integer  If assigned 1 it is an important code.

# Table: code_cat

**catid** integer  A unique auto-number.

**name** text  The name of the category.

**memo** text  Contains the memo text.

**owner** text  The coder who created the entry.

**date** text  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

**supercatid** integer  This represents the parent category of this category. It is Null if it is a top category.

# Table: code_image

**imgid** integer  A unique auto-number.

**id** integer  Links to the source.id to identify the source image file.

**x1** real  The left x position in pixels in the image file. Stored as decimal value.

**y1** real  The top y position in pixels in the image file. Stored as decimal value.

**width** real  The number of pixels across. Stored as decimal value.

**height** real The number of pixels down. Stored as decimal value.

**cid** integer  The code_name id to identify the code.

**memo** text  Contains the memo text.

**owner** text  The coder who created the entry.

**date** text  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

**important** integer  If assigned 1 it is an important code.

# Table: code_name

**cid** integer  A unique auto-number.

**name** text  The unique name of the code.

**memo** text  Contains the memo text.

**owner** text  The coder who created the entry.

**date** text  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

**color** text  A hex value ranging from '#000000' to '#FFFFFF' QualCoder recognises 120 colours so can apply light or dark text over the top. 

# Table: code_text

**ctid** integer  A unique auto-number.  (added in v3).

**cid** integer  The code_name id to link the code.

**fid** integer  The file source id to link the text file.

**seltext** text  A copy of the text of this coded text segment.

**pos0** integer  The starting character position in the text file. Null if not a text file.

**pos1** integer  The ending character position in the text file.  Null if not a text file.

**memo** text  Contains the memo text.

**owner** text  The coder who created the entry.

**date** text  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

**avid** integer  Link to a coded A/V segment time position. See table code_av.

**important** integer  If assigned 1 it is an important code.

# Table: journal

**jid** integer  A unique auto-number.

**name** text  Name of the journal.

**jentry** text  Contains the journal text.

**owner** text  The coder who created the entry.

**date** text  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

# Table: project

Should contain one row. Currently the current coder name is not in this table. In the future, I might add it here.

**databaseversion** text

**date** text  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

**memo** text  A memo about the overall project.

**about** text  Should describe the current QualCoder version used.  e.g. QualCoder 2.5

**bookmarkfile** integer  The id of the source text file. Used for jumping to the bookmark.

**bookmarkpos** integer  The character position in the text file. Used for jumping to the bookmark.

# Table: source

**id** integer  A unique auto-number.

**name** text

**fulltext** text  The fulltext of a text file, in UTF-8 encoding. Null if an image or A/V file.

**memo** text  Contains the memo text.

**owner** text  The coder who created the entry.

**date** text  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

**mediapath** text  

======

If the mediapath is empty it is an internally stored text file within the project folder.

If the mediapath begins with 'docs:' it is a link to an external text file. The fulltext will still be loaded into 'fulltext' for use.

If the mediapath begins with: '/images/' , '/audio/', '/video/' the image, audio or video file is stored internally in the project folder.

If the mediapath begins with: 'images:' , 'audio:', 'video:' the image, audio or video file is linked to externally. The full path to the file is stored.


