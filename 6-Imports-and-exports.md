Project menu
* Exports
* Imports

#  Codebook

This is an option under the Project Menu > Exports.

A codebook is a list of your codes. Each code memo should detail the reasons for the purpose of each code. The codebook can be exported to a text file. The codebook also shows the frequency of the codes used (from all coders). Example codebook output is shown below. As codes and categories are put in a tree like structure the double minus ‘–‘ indicates the subordinate codes and categories within a category.


#  REFI-QDA
The Rotterdam Exchange Format Initiative (REFI) is an open standard for exporting and importing codebooks and projects from and to different computer-aided qualitative data analysis software. The website for the exchange initiative is www.qdasoftware.org

Currently, QualCoder is able to export and import a codebook. 

_Exportation of a project and importation of a project are experimental and do not meet the full REFI-QDA standard. Some experimentation has been performed with Nvivo and MAXQDA qdpx files._

Importation of project.qpdx files seems to work with the test text-based projects. Features such as sets and graphs cannot be imported as this functionality is not within QualCoder. Other data formats are not preserved, for example date or boolean would be converted to text data. 

For audio and video, importation of transcriptions and syncpoints is untested. Importation/linking of relative linked files has not been tested.

To import, close any currently opened project first. Then choose a new QualCoder project name, then select the qdpx import file.

If no coded data is visible, you may need to change the current coder's name in Settings.Try the drop down coder name box.

# RQDA
Projects made with RQDA (http://rqda.r-forge.r-project.org/) can be directly imported. All data except for file categories are imported.

Close any opened project. Then in the Main Menu under Project click on RQDA Project import. You will be asked to create a new project- so enter a name. Then you will be asked to select the RQDA project file. QualCoder will then import the data.

If no coded data is visible, you may need to change the current coder's name in Settings. Tr ythe drop down coder name box.

# Survey import

This requires a CSV or Excel (xlsx format) file. You can try importing the survey.csv file in the Examples folder.

Survey files in a CSV format, are comma delimited, another delimiter can be chosen. For tab-delimited files type ta, tb, or tab in the Delimiter box so that QualCoder knows the csv file is tab delimited. **The first row must contain the headings for attributes. The first column must contain the unique identifiers for each survey respondent. **

QualCoder will determine if the other columns (attributes) are Numeric or Character. QualCoder cannot determine if an attribute is qualitative data. You must right-click and change the field type from character to qualitative for those fields that need to be qualitative. 

![Import survey dialog](https://qualcoder.files.wordpress.com/2020/10/import_survey.png?)

When you click on the OK button, the cases and their attributes will be added. The qualitative column will be converted to a file which will be named with the column name plus the current date and time. Each respondent's row will be prepended with [the unique id] so that you can identify each respondent. Also, the text for each respondent will be automatically linked to the corresponding case.

