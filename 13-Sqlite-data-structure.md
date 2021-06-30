The current v3 data structure is described to assist with developing sql queries. Tables are listed alphabetically.

# Table: annotation

**anid** _integer_  A unique auto-number

**fid** _integer_ Links to the source.id to identify the text file. Annotations are only for text files.

**pos0** _integer_  The starting character position in the text file.

**pos1** _integer_  The ending character position in the text file.

**memo** _text_  Contains the annotation text.

**owner** _text_  The coder who created the entry.

**date** _text_  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

# Table: attribute

**attrid** _integer_  A unique auto-number.

**name** _text_ The name of the attribute. This will match the name in attribute_type.

**attr_type** _text_  This is either 'case' or 'file'

**value** _text_ This store the attribute value as text, even if it is meant to be a numeric value. You may need to cast(value as real)

**id** _integer_ This field represents a source id or a case id.

**owner** _text_  The coder who created the entry.

**date** _text_  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

# Table: attribute_type

**name** _text_  The unique name of the attribute.

**owner** _text_  The coder who created the entry.

**date** _text_  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

**memo** _text_  Contains a memo about the attribute type.

**caseOrFile** _text_  This is either 'case' or 'file' 

**valuetype** _text_  This is either 'character' or 'numeric'

# Table: case_text

**id** _integer_ Unique autonumber.

**caseid** _integer_  Links to the cases.caseid.

**fid** _integer_ links to the source.id. These are only for text files.

**pos0** _integer_  The starting character position in the text file. Null if not a text file.

**pos1** _integer_  The ending character position in the text file.  Null if not a text file.

**memo** _text_  Contains the memo text.

**owner** _text_  The coder who created the entry.

**date** _text_  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

# Table: cases

**caseid** _integer_  A unique auto-number.

**name** _text_   The name of the case.

**memo** _text_  Contains the memo text.

**owner** _text_  The coder who created the entry.

**date** _text_  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

# Table: code_av

**avid** _integer_  A unique auto-number.

**id** _integer_  Links to the source.id to identify the source A/V file.

**pos0** _integer_  The starting milliseconds position in the A/V file.

**pos1** _integer_  The ending milliseconds position in the A/V file.

**cid** _integer_  The code_name id to identify the code.

**memo** _text_  Contains the memo text.

**owner** _text_  The coder who created the entry.

**date** _text_  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

**important** _integer_  If assigned 1 it is an important code.

# Table: code_cat

**catid** _integer_  A unique auto-number.

**name** _text_  The name of the category.

**memo** _text_  Contains the memo text.

**owner** _text_  The coder who created the entry.

**date** _text_  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

**supercatid** _integer_  This represents the parent category of this category. It is Null if it is a top category.

# Table: code_image

**imgid** _integer_  A unique auto-number.

**id** _integer_  Links to the source.id to identify the source image file.

**x1** _real_  The left x position in pixels in the image file. Stored as decimal value.

**y1** _real_  The top y position in pixels in the image file. Stored as decimal value.

**width** _real_  The number of pixels across. Stored as decimal value.

**height** _real_ The number of pixels down. Stored as decimal value.

**cid** _integer_  The code_name id to identify the code.

**memo** _text_  Contains the memo text.

**owner** _text_  The coder who created the entry.

**date** _text_  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

**important** _integer_  If assigned 1 it is an important code.

# Table: code_name

**cid** _integer_  A unique auto-number.

**catid** _integer_ The code_cat.catid if this code is part of a category. Null if not part of a category.

**name** _text_  The unique name of the code.

**memo** _text_  Contains the memo text.

**owner** _text_  The coder who created the entry.

**date** _text_  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

**color** _text_  A hex value ranging from '#000000' to '#FFFFFF' QualCoder recognises 120 colours so can apply light or dark text over the top. 

# Table: code_text

**ctid** _integer_  A unique auto-number.  (added in v3).

**cid** _integer_  The code_name id to link the code.

**fid** _integer_  The file source id to link the text file.

**seltext** _text_  A copy of the text of this coded text segment.

**pos0** _integer_  The starting character position in the text file. Null if not a text file.

**pos1** _integer_  The ending character position in the text file.  Null if not a text file.

**memo** _text_  Contains the memo text.

**owner** _text_  The coder who created the entry.

**date** _text_  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

**avid** _integer_  Link to a coded A/V segment time position. See table code_av.

**important** _integer_  If assigned 1 it is an important code.

# Table: journal

**jid** _integer_  A unique auto-number.

**name** _text_  Name of the journal.

**jentry** _text_  Contains the journal text.

**owner** _text_  The coder who created the entry.

**date** _text_  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

# Table: project

Should contain one row. Currently the current coder name is not in this table. In the future, I might add it here.

**databaseversion** _text_  Currently v1, v2 or v3. QualCoder will update to the most recent version (adds columns to tables).

**date** _text_  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

**memo** _text_  A memo about the overall project.

**about** _text_  Should describe the current QualCoder version used.  e.g. QualCoder 2.5

**bookmarkfile** _integer_  The id of the source text file. Used for jumping to the bookmark.

**bookmarkpos** _integer_  The character position in the text file. Used for jumping to the bookmark.

# Table: source

**id** _integer_  A unique auto-number.

**name** _text_  The name with fileextension of the file.  The file extension helps to determine if hte file is text, image or A/V. If the file has '.transcribed' as a suffix it is associated with the matching A/V file.

**fulltext** _text_  The fulltext of a text file, in UTF-8 encoding. Null if an image or A/V file.

**memo** _text_  Contains the memo text.

**owner** _text_  The coder who created the entry.

**date** _text_  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

**mediapath** _text_  



If the mediapath is empty it is an internally stored text file within the project folder.

If the mediapath begins with 'docs:' it is a link to an external text file. The fulltext will still be loaded into 'fulltext' for use.

If the mediapath begins with: '/images/' , '/audio/', '/video/' the image, audio or video file is stored internally in the project folder.

If the mediapath begins with: 'images:' , 'audio:', 'video:' the image, audio or video file is linked to externally. The full path to the file is stored.


