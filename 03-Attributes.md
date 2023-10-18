
# Attributes

Attributes are variables associated with files, cases or journals. They can be useful to add context to the text analysis. Open the Manage Attributes dialog. You can add, delete, rename and add memo notes to attributes.

You can right-click on a numeric attribute to convert to Character.

The only options for attributes are numeric and character. There are no options for boolean, date or time or specific numeric types such as integer.  However, if you are running SQL queries you may need to cast the numeric attribute to an Integer or Real: cast(my_var as integer).

Attributes to cases can be added in the Manage Cases section by clicking on the blue Plus button. Attributes to files can be added in the Manage Files section by clicking on he blue Plus button.
![Add attribute to files](https://qualcoder.files.wordpress.com/2022/07/add_file_attribute.png)

Attributes can be imported from a survey, and also from an REFI-QDA project file (REFI-QDA is experimental).

It is not the intention for QualCoder to perform statistical analyses of the attributes. It would be preferable to use dedicated statistical software such as R (https://www.r-project.org/) or other such software.

![Attributes dialog](https://qualcoder.files.wordpress.com/2020/12/manage_attributes.png)












