.. The COUNTER Code of Practice for Research Data © 2017-2024 by COUNTER Metrics
   is licensed under CC BY-SA 4.0. To view a copy of this license,
   visit https://creativecommons.org/licenses/by-sa/4.0/

Formats for Reports
===================

Code of Practice for Research Data Usage Metrics reports can be delivered in tabular form or as machine-readable JSON file via the SUSHI protocol. The tabular form MUST be a tab-separated-value Unicode text file. The machine-readable format MUST comply with the Research Data SUSHI API Specification (See Section 11).

All reports have the same layout and structure. Note that the Research Data SUSHI API Specification includes the same elements with the same or similar names; therefore, understanding the tabular reports translates to an understanding of what is REQUIRED in reports retrieved via SUSHI.

All reports have a header. In tabular reports, the header is separated from the body with a blank row. Beneath that is the body of the report with column headings. The contents of the body will vary by report. All of this is discussed in more detail below.


Report Header
"""""""""""""

The first 10 rows of a tabular report contain the header, and the 11th row is always blank. The COUNTER Code of Practice Release 5 rows Institution_Name and Institution_ID are not used. The header information is presented as a series of name-value pairs, with the names appearing in Column A and the corresponding values appearing in Column B. All tabular reports have the same names in Column A. Column B entries will vary by report.

Table 6.2 (below): Reports Header Elements

.. only:: latex

   .. tabularcolumns:: |>{\raggedright\arraybackslash}\Y{0.19}|>{\parskip=\tparskip}\Y{0.44}|>{\raggedright\arraybackslash}\Y{0.37}|

.. list-table::
   :class: longtable
   :widths: 13 54 33
   :header-rows: 1

   * - Element Name
     - Description of value to provide
     - Example

   * - Report_Name
     - The name of the report as it appears in Sections 6.1 and 6.2 of this document. Must be Dataset Report.
     - Dataset Report

   * - Report_ID
     - The unique identifier for the reports that is used in SUSHI requests.
     - dsr-12hd-zt65
     
   * - Release
     - The Code of Practice for Research Data Usage Metrics release this report complies with. Must be RD1.
     - RD1

   * - Metric_Types
     - A semicolon-space (“; “) delimited list of metric types requested for this report. Note that even though a Metric Type was requested, it might not be included in the body of the report if no report items had usage of that type.
     - Unique_Dataset_Investigations; Unique_Dataset_Requests

   * - Report_Filters
     - A series of zero or more report filters applied on the reported usage, excluding metric types (which appear in a separate row). Typically, a report filter affects the amount of usage reported. Entries appear in the form of “filter_Name=filter_Value” with multiple filter name-value pairs separated with a semicolon-space (“; “) and multiple filter values for a single filter name separated by the vertical pipe (“|”) character.
     - Access_Method=Regular; Access_Method_Machine

   * - Report_Attributes
     - A series of zero or more report attributes applied to the report. Typically, a report attribute affects how the usage is presented but does not change the numbers.
       Entries appear in the form of “attribute_name=attribute_value” with multiple attribute name-value pairs separated with a semicolon-space (”; ”) and multiple attribute values for a single attribute name separated by the vertical pipe (“|”) character.
     - Attributes_To_Show=Access_Method
     
   * - Exceptions
     - An indication of some difference between the usage that was created and the usage that is being presented in the report. The format for the exception values are: “Error_No: Exception_Description” (Data). The **Error_No** and **Exception_Description** MUST match values provided in Table B.1 of Appendix B. The data is OPTIONAL.
       Note that for tabular reports, only the limited set of exceptions where usage is returned will apply.
     - 3040: Partial Data Returned (request was for 2016-01-01 to 2016-12-31; however, usage is only available to 2016-08-30).
       3040: Partial Data Returned
          
   * - Reporting_Period
     - The date range for the usage represented in the report, in the form of: “begin_date=yyyy-mm-dd”; “end_date=yyyy-mm-dd”. Should conform with ISO 8601 (ISO 8601:2004 – Data elements and interchange formats, 2004).
       The begin_date MUST be the first day of the month, whereas the end_date can be the last day of the month for a complete monthly report, or any other day in the month for a partial monthly report (See Section 6.3.6).
     - begin_date=2016-01-01; end_date=2016-08-30
     
   * - Created
     - The date the usage was prepared, in the form of “yyyy-mm-dd” according to ISO 8601 (ISO 8601:2004 – Data elements and interchange formats, 2004).
     - 2016-10-11
     
   * - Created_By
     - The name of the organization or system that created the report.
     - DataONE
     
   * - (blank row)
     - Row 11 MUST be blank.
     - 
