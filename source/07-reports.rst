.. The COUNTER Code of Practice for Research Data © 2017-2024 by COUNTER Metrics
   is licensed under CC BY-SA 4.0. To view a copy of this license,
   visit https://creativecommons.org/licenses/by-sa/4.0/

Dataset Reports
===============

Dataset reports provide a summary of activity related to a dataset and provide a means of evaluating the reuse of that dataset.

Table 7.1 (below): Dataset Master Report and Standard Views

.. only:: latex

   .. tabularcolumns:: |>{\raggedright\arraybackslash}\Y{0.13}|>{\raggedright\arraybackslash}\Y{0.17}|>{\parskip=\tparskip}\Y{0.37}|>{\raggedright\arraybackslash}\Y{0.33}|

.. list-table::
   :class: longtable
   :widths: 10 18 48 24
   :header-rows: 1

   * - Report_ID
     - Report_Name
     - Details
     - Host_Types

   * - DSR
     - Dataset Master Report
     - A granular customizable report showing activity at the level of the dataset that allows the user to apply filters and select configuration options.
     - Repository\ |br|\ |lb|
       Data Repository


Report Header
"""""""""""""

Table 7.2 shows the header details for the Dataset Master Report which contain additional filters and breakdowns beyond those included in the standard COUNTER reports, and are reported at the Dataset level, and its Standard Views.

For the tabular reports, elements MUST appear in the exact order shown, and spelling, casing and punctuation of labels (Column A) and fixed data elements such as report names (Column B) MUST match exactly. The SUSHI version of the report MUST comply with the Report_Header definition in the Research Data SUSHI API Specification (see Section 8). Entries in the table appearing in italics describe the values to include.

Table 7.2 (below): Header for Dataset Master Report and Standard Views

.. only:: latex

   .. tabularcolumns:: |>{\raggedright\arraybackslash}\Y{0.1}|>{\parskip=\tparskip}\Y{0.35}|>{\raggedright\arraybackslash}\Y{0.55}|

.. list-table::
   :class: longtable
   :widths: 10 30 60
   :header-rows: 1

   * - Row
     - Label for Tabular Report (column A)
     - Value for Tabular Report (column B)

   * - 1
     - Report_Name
     - Dataset Master Report

   * - 2
     - Report_ID
     - DSR

   * - 3
     - Release
     - RD1

   * - 4
     - Metric_Types
     - Semicolon-space delimited list of metric types included in the report

   * - 5
     - Report_Filters
     - Semicolon-space delimited list of filters applied to the data to generate the report

   * - 6
     - Report_Attributes
     - Semicolon-space delimited list of report attributes applied to the data to generate the report

   * - 7
     - Exceptions
     - Any exceptions that occurred in generating the report, in the format “Error_Number: Error_Description”

   * - 8
     - Reporting_Period
     - Date range requested for the report in the form of “yyyy-mm-dd” to “yyyy-mm-dd”. The “dd” of the from-date is 01. The “dd” of the to-date can be the last day of the to- month, or another day of the to-month, in which case the reporting with be partial for that month.

   * - 9
     - Created
     - Date the report was run in the format of “yyyy-mm-dd”

   * - 10
     - Created_By
     - Name of organization or system that generated the report

   * - 11
     - (blank)
     - (blank)


Column Headings/Elements
""""""""""""""""""""""""

When applicable, the following elements MUST appear in the tabular report in the order they appear in Table 7.3. For guidance on how these fields appear in the JSON format, refer to the Research Data SUSHI API Specification (see Section 8).

Table 7.3 (below): Column Headings/Elements for Dataset Master Report and Standard Views

.. only:: latex

   .. tabularcolumns:: |>{\raggedright\arraybackslash}\Y{0.30}|>{\raggedright\arraybackslash}\Y{0.1}|

.. list-table::
   :class: longtable
   :widths: 30 10
   :header-rows: 1

   * - Field name (Tabular)
     - DSR

   * - Dataset_Title
     - M

   * - Publisher
     - M

   * - Publisher_ID
     - M

   * - Creators
     - O

   * - Publication_Date
     - O

   * - Dataset_Version
     - O

   * - DOI
     - M*

   * - Other_ID
     - M*

   * - URI
     - M*

   * - YOP
     - O

   * - Access_Method
     - O

   * - Metric_Type
     - M

   * - Reporting_Period_Total
     - M

   * - mmm-yyyy
     - M

\* The tabular report MUST either include DOI, OTHER_ID or URL.


Filters and Attributes
""""""""""""""""""""""

Table 7.4 presents the values that can be chosen for the Dataset Master Report and that are pre-set for the Standard Views.

Table 7.4 (below): Filters/Attributes for Dataset Master Report and Standard Views

.. only:: latex

   .. tabularcolumns:: |>{\raggedright\arraybackslash}\Y{0.3}|>{\parskip=\tparskip}\Y{0.7}|

.. list-table::
   :class: longtable
   :widths: 30 70
   :header-rows: 1

   * - Filter/Attribute
     - DSR

   * - YOP
     - All years, a specific year, or a range of years. Use “0001” for unknown.

   * - Access_Method
     - One or all of Regular or Machine

   * - Version
     - Either “All” or a specific version, e.g. “1.3”.

   * - Metric Type
     - One or more of:\ |br|\ |lb|
       Total_Dataset_Investigations\ |br|\ |lb|
       Total_Dataset_Requests\ |br|\ |lb|
       Unique_Dataset_Investigations\ |br|\ |lb|
       Unique_Dataset_Requests

   * - Exclude_Monthly_Details
     - Either “True” or “False”.

If a filter is applied to a column that doesn’t show on the report, usage for all selected attribute values is summed and the totals are presented in the report.

