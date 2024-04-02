.. The COUNTER Code of Practice for Research Data © 2017-2024 by COUNTER Metrics
   is licensed under CC BY-SA 4.0. To view a copy of this license,
   visit https://creativecommons.org/licenses/by-sa/4.0/

Delivery of Reports
===================

Content providers MUST make tabular versions of reports available from an administrative/reporting site. All reports provided by the content provider MUST also be available via SUSHI protocols. Delivery requirements are:

* Reports MUST be provided in both of the following formats:

  * Tab Separated Value (TSV) file that can be easily imported into spreadsheet programs such as Microsoft Excel without loss or corruption of data.
  * JSON formatted in accordance with the Research Data SUSHI API Specification (Research Data SUSHI API Specification, 2018).
* Each report MUST be delivered as a separate file to facilitate automated processing of usage reports.
* Tabular reports MUST be made available through a website.

  * The website MAY be password-controlled.
  * Email alerts MAY be sent when data is updated.
  * The report interface MUST provide filter and configuration options for the Master Reports that apply to the content provider.
  * The report interface MUST offer all Standard Views that apply to the content provider’s host type(s) and Standard View options MUST automatically apply the REQUIRED filter and configuration options and not allow the user to alter the filters or configuration options except for the usage begin and end dates.
  * The date range fields on the user interface SHOULD default to the latest month with complete usage. For example, if the current date is 15 May 2019 and April usage has been processed, the begin date would default to 01 April 2019 and the end date would default to 30 April 2019. If the April usage has not yet been processed, the start and end dates would default to 01 March 2019 to 31 March 2019. If the May usage has already been processed partially, the begin date would default to 01 April 2019 and the end date would default to the date until which usage has been processed, e.g. 10 May 2019.
  * Master Reports must include the option to Exclude_Monthly_Details. When selected, the monthly columns are excluded from the report (only ReportingPeriod Totals appear). Note: this option is NOT available for reports retrieved via SUSHI; however, SUSHI does offer a Granularity Report Attribute that allows usage to be retrieved with a granularity of month, year, or totals.
* Reports MUST be provided monthly.
* Data MUST be updated within 1 month of the end of the reporting period.
* Usage MAY be processed for the entire month before usage for that month is included in reports. If usage for a full given month is not yet available, partial usage for that month MAY be returned.
* A minimum of the current year plus the prior most recent 24 months of usage data MUST be available, or the period that reports have been generated according to the Code of Practice for Research Data Usage Metrics if that period is shorter than 24 months.
* The reports MUST allow the customer the flexibility to specify a date range, in terms of months, within the most recent 24-month period. Where no date range is specified, the default MUST be calendar year and calendar-year-to-date reports for the current year.
* Reports MUST be available for harvesting via the SUSHI protocol within 1 month of the end of the reporting period.
