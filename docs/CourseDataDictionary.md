# Course Data Dictionary
__Bridget Weill & Chris Lametta__


## Class
| Key | Field | Definition | Type |
| :--- | :--- | :--- | :--- |
| PK | ClassID | | Integer |
| FK | CourseCatalogID | | Integer |
| FK | ProfessorID | | Integer |
| | CatalogID | |Text |
| | Term | | Text |
| | CRN | | Integer |
| | Section | | Integer |
| | Credits | | Integer |
| | Title | | Text |
| | Timecodes | | Text |
| | Meetings | | Text |
| | Capacity | | Integer |
| | Actual | | Integer |
| | Remaining | | Integer |

## CourseCatalog
| Key | Field | Definition | Type |
| :--- | :--- | :--- | :--- |
| PK | CourseCatalogID | | Integer |
| FK | ProgramID | | Integer |
| | CatalogID | | Text |
| | Catalog_Year | | Text |
| | Title | | Text |
| | Credits | | Text |
| | Prereqs | | Text |
| | Coreqs | | Text |
| | Fees | | Text |
| | Attributes | | Text |
| | Description | | Text |

## Meeting
| Key | Field | Definition | Type |
| :--- | :--- | :--- | :--- |
| PK | MeetingID | | Integer |
| FK | ClassID | | Integer |
| FK | LocationID | | Integer |
| | Day | |Text |
| | StartTime | | Text |
| | EndTime | | Text |

## Program
| Key | Field | Definition | Type |
| :--- | :--- | :--- | :--- |
| PK | ProgramID | | Integer |
| FK | Program_Name | | Text |
| FK | Program_Code | | Text |

## Location
| Key | Field | Definition | Type |
| :--- | :--- | :--- | :--- |
| PK | LocationID | | Integer |
| | Location | | Text |

## Professors
| Key | Field | Definition | Type |
| :--- | :--- | :--- | :--- |
| PK | ProfessorID | | Integer |
| | Name | | Text |

__2. Design a normalized relational database that can contain all CSV data in your `SourceData` repository. Document the design with an ERD and a data dictionary.__

- The database should not leave off any files or columns.
- Normalize to at least BCNF.
- The ERD should be a PDF file named "CourseDataERD.PDF" to be dropped in the `docs` folder.
- Also in the `docs` folder, add a Markdown-formatted `CourseDataDictionary.md` file that defines every column on every table. Use the table names as second level headings (`##`) and bullet lists for the column definitions. If you are feeling frisky, then perhaps use Markdown tables instead of bullet lists.  
- Take care with the [Markdown formatting](https://github.github.com/gfm/). Dropping big, stupidly-formatted blobs of text is very bad form. It's also extremely unprofessional.

