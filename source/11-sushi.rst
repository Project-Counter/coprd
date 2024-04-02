.. The COUNTER Code of Practice for Research Data © 2017-2024 by COUNTER Metrics
   is licensed under CC BY-SA 4.0. To view a copy of this license,
   visit https://creativecommons.org/licenses/by-sa/4.0/

SUSHI for Automated Report Harvesting
=====================================

Content providers MUST support automatic harvesting of reports via the SUSHI protocol as described in the NISO SUSHI Protocol (ANSI/NISO Z39.93-2014: Standardized Usage Statistics Harvesting Initiative (SUSHI) Protocol, 2014) and the Research Data SUSHI API Specification (Research Data SUSHI API Specification, 2018).


Research Data SUSHI API Paths to Support
""""""""""""""""""""""""""""""""""""""""

The following paths (methods) MUST be supported:

Table 8.1 (below): Research Data SUSHI API Paths

.. only:: latex

   .. tabularcolumns:: |>{\raggedright\arraybackslash}\Y{0.13}|>{\raggedright\arraybackslash}\Y{0.17}|>{\parskip=\tparskip}\Y{0.37}|>{\raggedright\arraybackslash}\Y{0.33}|

.. list-table::
   :class: longtable
   :widths: 10 18 48 24
   :header-rows: 1

   * - Path
     - Description

   * - GET /status
     - Returns the current status of the Research Data SUSHI API service. This path returns a message that includes the operating status of the API, the URL to the service’s entry in the Register of Compliant Content Providers, and an array of service alerts (if any).

   * - GET /reports
     - Returns a list of reports supported by the Research Data SUSHI API service. The response includes an array of reports, including the report identifier, the release number, the report name, a description, a list of supported report filters, and a list of supported report attributes.

   * - GET /reports/{ReportID}
     - Each supported report has its own path, e.g. GET /reports/DSR for dataset requests.


Authentication and Security for the Research Data SUSHI API
"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""

The Research Data SUSHI API SHOULD be implemented using TLS (HTTPS). The Research Data SUSHI API MAY be secured using an API key or username/password assigned to the organization harvesting the usage.


Report Filters and Report Attributes
""""""""""""""""""""""""""""""""""""

The Research Data SUSHI API Specification allows report responses to be customized to the caller’s needs using report filters and report attributes. These filters and attributes are implicit for Standard Views. Filters and attributes are explicitly included as parameters on the Research Data SUSHI API request for Master Reports. Refer to (Research Data SUSHI API Specification, 2018) for the list of filters and attributes supported by the various reports.


Research Data SUSHI API Errors and Exceptions
"""""""""""""""""""""""""""""""""""""""""""""

Implementations of the Research Data SUSHI API MUST comply with the warnings, exceptions and errors described in the Research Data SUSHI API Specification. See Appendix B.


SUSHI Service Limits
""""""""""""""""""""

The content provider MUST NOT place limits on the SUSHI service (such as requests per day or amount of data transferred) that would prevent users from retrieving reports.
