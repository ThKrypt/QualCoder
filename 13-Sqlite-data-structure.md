The current v3 data structure is described to assist with developing sql queries. Tables are listed alphabetically.

**Table: annotation**

anid integer  A unique auto-number

fid integer links to the source.id. These are only for text files.

pos0 integer  The starting character position in the text file.

pos1 integer  The ending character position in the text file.

memo text  Contains the annotation text.

owner text  The coder who created the entry.

date text  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

**Table: attribute**

attrid

name

attr_type

value

id

owner text  The coder who created the entry.

date text  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

**Table: attribute_type**

name

owner text  The coder who created the entry.

date text  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

memo text  Contains a memo about the attribute type.

caseOrFile

valuetype

**Table: case_text**

id integer Unique autonumber.

caseid integer  Links to the cases.caseid.

fid integer links to the source.id. These are only for text files.

pos0 integer  The starting character position in the text file. Null if not a text file.

pos1 integer  The ending character position in the text file.  Null if not a text file.

memo text  Contains the memo text.

owner text  The coder who created the entry.

date text  The date and time the entry was created, format yyyy-mm-dd hh:mm:ss

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


