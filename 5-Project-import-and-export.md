Project menu
* Exports
* Imports

#  Codebook

This is an option under the Project Menu > Exports.

A codebook is a list of your codes. Each code memo should detail the reasons for the purpose of each code. The codebook can be exported to a text file. The codebook also shows the frequency of the codes used (from all coders). Example codebook output is shown below. As codes and categories are put in a tree like structure the double minus ‘–‘ indicates the subordinate codes and categories within a category.


#  REFI-QDA
The Rotterdam Exchange Format Initiative (REFI) is an open standard for exporting and importing codebooks and projects from and to different computer-aided qualitative data analysis software. The website for the exchange initiative is www.qdasoftware.org

Currently, QualCoder is able to export and import a codebook. Exportation of a project and importation of a project are experimental and do not meet the full REFI-QDA standard. For example: greater than 2GB files are not stored externally on export. Some experimentation has been performed with Nvivo and MAXQDA qdpx files.

Importation of project.qpdx files partly works, coding stripes may not correctly match text selections (sometimes may be off by a character). External files greater than 2GB may not be imported into QualCoder project. Features such as sets and graphs cannot be imported as this functionality is not withing QualCoder. Other data formats are not preserved, for example date or boolean would be converted to text data. 

To import, close any currently opened project first. Then choose a new QualCoder project name, then select the qdpx import file.

If no coded data is visible, you may need to change the current coder's name in Settings.Try the drop down box.

# RQDA
Projects made with RQDA (http://rqda.r-forge.r-project.org/) can be directly imported. All data except for file categories are imported.

Close any opened project. Then in the Main Menu under Project click on RQDA Project import. You will be asked to create a new project- so enter a name. Then you will be asked to select the RQDA project file. QualCoder will then import the data.

If no coded data is visible, you may need to change the current coder's name in Settings.

# Survey Import

Importing surveys in csv and Excel (xlsx format) are available under the imports menu. Detailed instructions on importing surveys are on page 2 of the wiki: _2 Files, Cases, Attributes, Survey import_