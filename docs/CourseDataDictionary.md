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
| | CRN | Course Registration Number: Specific to an individual class | Integer |
| | Section | | Integer |
| | Credits | The recognition for having taken a course at school or university; measures if enough hours have been made for graduation | Integer |
| | Title | Name of the class | Text |
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


- Also in the `docs` folder, add a Markdown-formatted `CourseDataDictionary.md` file that defines every column on every table. Use the table names as second level headings (`##`) and bullet lists for the column definitions. If you are feeling frisky, then perhaps use Markdown tables instead of bullet lists.  
- Take care with the [Markdown formatting](https://github.github.com/gfm/). Dropping big, stupidly-formatted blobs of text is very bad form. It's also extremely unprofessional.

