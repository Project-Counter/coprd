.. The COUNTER Code of Practice for Research Data © 2017-2024 by COUNTER Metrics
   is licensed under CC BY-SA 4.0. To view a copy of this license,
   visit https://creativecommons.org/licenses/by-sa/4.0/

Report Common Attributes and Elements
=====================================

COUNTER Code of Practice Release 5 introduced several new elements and attributes in order to help organize the information in a single, consistent, and coherent Code of Practice. The Code of Practice for Research Data Usage Metrics uses a subset of these elements and attributes relevant for research data.


Host Types
""""""""""

Research data usage reports are provided by different types of content hosts, and the usage reporting needs vary by host type. Although the “Host Type” does not appear on the report, the Code of Practice uses “Host Types” throughout this document to help content providers identify which reports, elements, metric types, and attributes are relevant to them.

The Code of Practice for Research Data Usage Metrics uses the following host types:

Table 6.3 (below): List of Host Types

.. only:: latex

   .. tabularcolumns:: |>{\raggedright\arraybackslash}\Y{0.2}|>{\raggedright\arraybackslash}\Y{0.55}|>{\parskip=\tparskip}\Y{0.25}|

.. list-table::
   :class: longtable
   :widths: 20 55 25
   :header-rows: 1

   * - Host Type Category
     - Description
     - Example

   * - Repository
     - A repository that hosts multiple research output types including research data. Institutional repositories are typically in this category.
     - Figshare

   * - Data Repository
     - A research data repository hosting only research data. Disciplinary repositories are typically in this category.
     - CDL Dash, Dryad Digital Repository


Data Types
""""""""""

The COUNTER Code of Practice Release 5 reports scholarly information in many ways. These major groupings are referred to as Data Types. Only the Dataset Data Types are used by the Code of Practice for Research Data Usage Metrics. Reporting of collections is restricted to pre-set collections that are defined like databases.

Table 6.4 (below): List of Data Types

.. only:: latex

   .. tabularcolumns:: |>{\raggedright\arraybackslash}\Y{0.13}|>{\raggedright\arraybackslash}\Y{0.17}|>{\parskip=\tparskip}\Y{0.37}|>{\raggedright\arraybackslash}\Y{0.33}|

.. list-table::
   :class: longtable
   :widths: 10 18 48 24
   :header-rows: 1

   * - Data Type
     - Description
     - Host Types
     - Reports (abbrev)

   * - Dataset
     - A dataset.
     - Repository
       Data Repository
     - DSR


Metric Types
""""""""""""

The following metric types are defined to enable reporting. There is no significant difference to the COUNTER Code of Practice Release 5.

**Investigations and Requests of Items and Titles**

This group of Metric Types represents activities where datasets were retrieved (Requests) or information about a dataset (e.g. metadata) was examined (Investigations).  Any user activity that can be attributed to a Dataset will be considered an Investigation, including downloading or viewing the Dataset. Requests are limited to user activity related to retrieving or viewing the Dataset itself.

**Total_Dataset, Unique_Dataset**

The metric types that begin with Total\_ mean that if a dataset was accessed multiple times in a user session, the metric would increase by the number of times the Dataset was accessed (minus any adjustments for double-clicks).

Unique_Dataset metrics help eliminate the effect different styles of user interface may have on usage counts. If the same dataset was accessed multiple times in a given user session, the corresponding metric can only increase by 1 to simply indicate that the dataset was accessed in the session.

Table 6.5 (below): List of Metric Types

.. only:: latex

   .. tabularcolumns:: |>{\raggedright\arraybackslash}\Y{0.3}|>{\raggedright\arraybackslash}\Y{0.41}|>{\parskip=\tparskip}\Y{0.19}|>{\raggedright\arraybackslash}\Y{0.1}|

.. list-table::
   :class: longtable
   :widths: 25 48 17 10
   :header-rows: 1

   * - Metric Type
     - Description
     - Host Types
     - Reports (abbrev)

   * - Total_Dataset_Investigations
     - Total number of times a Dataset or information related to a Dataset was accessed and the data volume in megabytes that was transferred. Double click filters are applied to these transactions. Investigations (counts and volume) are reported for each version of the Dataset and for the cumulative total across versions.
     - Repository\ |br|\ |lb|
       Data Repository
     - DSR
     
   * - Unique_Dataset_Investigations
     - Number of datasets investigated in unique user-sessions. If investigations for multiple components of the same Dataset occur in the same user-session, there MUST be only one “unique” activity counted for that Dataset. Investigations (counts and volume) are reported for each version of the Dataset and for the cumulative total across versions.
     - Repository\ |br|\ |lb|
       Data Repository
     - DSR
     
   * - Total_Dataset_Requests
     - Total number of times a Dataset was retrieved (the content was accessed or downloaded in full or a section of it) and the data volume in megabytes that was transferred. Double-click filters applied. Requests (counts and volume) are reported for each version of the Dataset and for the cumulative total across versions.
     - Repository\ |br|\ |lb|
       Data Repository
     - DSR
     
   * - Unique_Dataset_Requests
     - Number and data volume of Datasets requested in unique user-sessions. If requests for multiple components of the same Dataset occur in the same user-session, there MUST be only one “unique” activity counted for that Dataset. Requests (counts and volume) are reported for each version of the Dataset and for the cumulative total across versions.
     - Repository\ |br|\ |lb|
       Data Repository
     - DSR


Access Methods
""""""""""""""

In order to track content usage by machines, and to keep that usage separate from regular usage by humans, the Access_Method attribute is used.

Table 6.6 (below): List of Access Methods

.. only:: latex

   .. tabularcolumns:: |>{\raggedright\arraybackslash}\Y{0.17}|>{\raggedright\arraybackslash}\Y{0.54}|>{\parskip=\tparskip}\Y{0.19}|>{\raggedright\arraybackslash}\Y{0.1}|

.. list-table::
   :class: longtable
   :widths: 17 54 19 10
   :header-rows: 1

   * - Access Method
     - Description
     - Host Types
     - Reports (abbrev)

   * - Regular
     - Refers to activities on a platform or content host that represent typical user behavior.
     - Repository\ |br|\ |lb|
       Data Repository
     - DSR
     
   * - Machine
     - Refers to activities on a platform or content host that represent typical machine behavior. This includes only legitimate machine access and excludes internet robots and crawlers (see Section 10.5).
     - Repository\ |br|\ |lb|
       Data Repository
     - DSR


Year of Publication (YOP)
""""""""""""""""""""""""""

Analyzing collection usage by the age of the content is also desired. The “YOP” usage attribute represents year of publication.

Table 6.7 (below): Year of Publication Formatting

.. only:: latex

   .. tabularcolumns:: |>{\raggedright\arraybackslash}\Y{0.1}|>{\raggedright\arraybackslash}\Y{0.61}|>{\parskip=\tparskip}\Y{0.19}|>{\raggedright\arraybackslash}\Y{0.1}|

.. list-table::
   :class: longtable
   :widths: 10 61 19 10
   :header-rows: 1

   * - YOP
     - Description
     - Host Types
     - Reports (abbrev)

   * - yyyy
     - The Year of Publication for the item as a four-digit year. If the year of publication is not known, use a value of 0001.
     - Repository\ |br|\ |lb|
       Data Repository
     - DSR


Partial Monthly Reports
"""""""""""""""""""""""

The Reporting_Period can end before the last day of the month, in which case the report for that month will be partial. This enables incremental updates of usage reporting during the course of a month. These incremental updates always replace the previous report for that month. Reporting of usage broken down by day is not supported in this release of the Code of Practice for Research Data Usage Metrics.


Zero Usage
""""""""""

Inclusion of zero-usage reporting for everything, including unsubscribed content, could make reports unmanageably large.

* For tabular reports

  * Omit any row where the Reporting Period Total would be zero.
  * If the Reporting Period Total is >0, but usage for an included month is zero, set the cell value for that month to 0.
* For SUSHI version of reports

  * Omit any Instance element with a count of zero.
  * Omit Performance elements that don’t have at least one Instance
  * Omit ReportItems elements that don’t have at least one Performance


Missing and Unknown Field Values
""""""""""""""""""""""""""""""""

* For tabular reports

  * If a field value is missing or unknown (i.e. the DOI for an item doesn’t exist or isn’t known), the field MUST be left blank. For clarity, the field MUST NOT contain values such as “unknown” or “n/a”.
* For SUSHI version of reports

  * If the value of a field is missing or unknown and the Research Data SUSHI API Specification (see Section 11) indicates the field is REQUIRED, the value of the field MUST be expressed as empty as appropriate for the data type.
  * If the value of a field is missing or unknown and the field is not REQUIRED according to the Research Data SUSHI API Specification, the field MUST be omitted from the response.
