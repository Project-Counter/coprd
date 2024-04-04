.. The COUNTER Code of Practice for Research Data © 2017-2024 by COUNTER Metrics
   is licensed under CC BY-SA 4.0. To view a copy of this license,
   visit https://creativecommons.org/licenses/by-sa/4.0/

Introduction
===================

This is the first version of a Code of Practice for Research Data. The purpose of this report is to enable data repositories and platform providers to produce consistent, comparable, and credible usage metrics for research data. This first release of the Code of Practice for Research Data Usage Metrics has been kept intentionally narrow in scope to focus on the dataset level and avoid creating unnecessary hurdles to adoption.


Purpose
"""""""

The purpose of the Code of Practice for Research Data Usage Metrics is to facilitate the recording, exchange, and interpretation of online usage data by establishing open standards and protocols for the provision of content-provider-generated usage statistics that are consistent, comparable, and credible.


Scope
"""""

This Code of Practice for Research Data Usage Metrics is aligned with the COUNTER Code of Practice Release 5 (https://cop5.projectcounter.org/en/5.0.3/) and provides a framework for recording and exchanging online usage statistics for research data at an international level. It covers the following areas: data elements to be measured; definitions of these data elements; content and format of usage reports; requirements for data processing; and guidelines to avoid duplicate counting.


Relationship to COUNTER Code of Practice Release 5
""""""""""""""""""""""""""""""""""""""""""""""""""

Developed by members from the research data management community (RDM) in close coordination with COUNTER, this Code of Practice for Research Data follows the COUNTER Code of Practice Release 5 (COUNTER Code of Practice Release 5, 2017) recommendations as much as possible (where relevant) and deviates from them only when necessary.

There are different use cases and practices between research data and the majority of scholarly resources. For example, research data does not need to be reported at the institutional level, but geographic aggregation may be important. Another significant difference is the need for aggregation of usage across components for all versions of a dataset. It is common practice for research data to be versioned, and we recommend reporting the usage data for each specific version and the combined usage for all versions.

The first release of the Code of Practice for Research Data Usage Metrics only describes reporting of usage at the dataset level. For future releases, reporting usage statistics for dataset components will be considered based on community feedback. Following the COUNTER Code of Practice Release 5, standard usage statistics are not reported by format distribution, e.g., no separate numbers for downloads in CSV and XLSX formats.

Download volume (i.e., file size) can be reported. There are widely varying practices in the research data community regarding the granularity and structure of datasets, components, and collections. Reporting download volume makes it easier to compare usage for research data packaged into datasets with different granularity.

Geolocation information and country are reported, but not IP addresses. For large countries (e.g. United States) reporting at the state or province level may be enabled. Reporting of geolocation information helps to better understand usage for the same datasets hosted in multiple locations, and for datasets where usage is dependent upon the location of the user, e.g., datasets describing research in a particular geolocation.

Usage metrics are reported for each specific version of a dataset, as well as the combined usage for all versions. Usage metrics are only reported for individual datasets. In this version of the Code of Practice for Research Data Usage Metrics there is no report format for reporting usage for collections of datasets, for example all datasets in a data repository.


Strategy
""""""""
The Code of Practice for Research Data Usage Metrics will evolve in response to the demands of the international library, data management, and content provider communities. The Code of Practice for Research Data Usage Metrics is continually under review; feedback on its scope and application are actively sought from all interested parties.


Governance
""""""""""

The Code of Practice for Research Data Usage Metrics is developed by the Make Data Count project (Make Data Count, 2017), in close collaboration with Counter Online Metrics (COUNTER) (Project COUNTER, 2002), a non-profit organization that maintains the COUNTER Code of Practice.


Definitions
"""""""""""

This Code of Practice for Research Data Usage Metrics provides definitions of data elements and other terms that are relevant not only to the usage reports specified in this document, but also to other reports that content providers may wish to generate. Every effort has been made to use existing COUNTER, ISO, NISO, etc. definitions where appropriate, and these sources are cited (see References and Appendix A). The following key definitions are used by the Code of Practice for Research Data Usage Metrics:

* Dataset: An aggregation of data, published or curated by a single agent, and available for access or download in one or more formats, with accompanying metadata (Dekkers & Isaac, 2018). A dataset is a subtype of a COUNTER content item. Synonymous term: data package.
* Component: Part of the data available for a dataset that can be accessed or downloaded individually. Aligns with a COUNTER component. Synonymous terms: data file, data granule.
* Collection: A curated aggregation of datasets. Related terms: catalog, repository.
* Version: Multiple versions of a dataset are defined as significant changes to the content and/or metadata, associated with changes in one or more components, and that would result in changes to fixity attributes of the components.


Versions
""""""""

The Code of Practice for Research Data Usage Metrics will be extended and upgraded as necessary, based on input from the communities it serves. Future versions might be integrated into the COUNTER Code of Practice. A continuous maintenance process will allow the Code of Practice for Research Data Usage Metrics to evolve over time minimizing the need for major version changes.


Auditing and Code of Practice for Research Data Usage Metrics Compliance
""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""

No content provider following the Code of Practice for Research Data Usage Metrics has been audited at the time of this first release of the Code of Practice for Research Data Usage Metrics.

While we expect the auditing process for research data usage reporting to be similar to audits in the context of the COUNTER Code of Practice Release 5, it is not yet known which organizations are willing to perform audits according to the Code of Practice for Research Data Usage Metrics, and how these audits differ from COUNTER Code of Practice Release 5 audits. For these reasons audits for research data usage reporting according to the Code of Practice for Research Data Usage Metrics are not required at this point in time.


Privacy and User Confidentiality
""""""""""""""""""""""""""""""""

Statistical reports or data that reveal information about individual users will not be released or sold by content providers without the permission of that individual user, the consortium, and its member institutions (ICOLC Guidelines for Statistical Measures of Usage of Web-Based Information Resources (1998, revised 2001, 2006), 2006).


Relationship to Other Standards, Protocols and Codes
"""""""""""""""""""""""""""""""""""""""""""""""""""""

The Code of Practice for Research Data Usage Metrics builds on several existing industry initiatives and standards that address content provider-based online performance measures. In addition to the COUNTER Code of Practice this includes the Scholix Metadata Schema for the Exchange of Scholarly Communication Links (Burton et al., 2017) and the NISO Alternative Assessment Metrics Project (NISO RP-25-2016: Outputs of the NISO Alternative Assessment Metrics Project, 2016).

Where appropriate, definitions of data elements and other terms from these sources have been used in this Code of Practice for Research Data Usage Metrics, and these are identified in Appendix A.


Changes from Previous Versions
""""""""""""""""""""""""""""""

This is the first release of the Code of Practice for Research Data Usage Metrics.