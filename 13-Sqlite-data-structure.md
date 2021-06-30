The current v3 data structure is described to assist with developing sql queries.

**Table: annotation**

anid integer  A unique auto-number

fid integer links to the source.id. These are only for text files.

pos0 integer  The starting character position in the text file.

pos1 integer  The ending character position in the text file.

memo text  Contains the annotation text.

owner text  The coder who created the entry.

date text  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

**Table: attribute**

**Table: attribute_type**

**Table: case_text**

**Table: cases**

**Table: code_av**

**Table: code_cat**

**Table: code_image**

**Table: code_name**

**Table: code_text**

**Table: journal**

**Table: links_type**

**Table: project**

**Table: source**


