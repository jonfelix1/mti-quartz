---
tags:
- mandat
- topic
- note
Class: "[[Data Management Class (ManDat)]]"
Topic: "[[Data Architecture]]"
---

# Data Delivery Architecture

Data Delivery Architecture encompasses various components that ensure effective integration, management, and utilization of data across an organization. This architecture includes several key elements, such as data integration, database architecture, unstructured information architecture, and metadata architecture.

## Data Integration Architecture

> DW/BI Architecture
> ![[Pasted image 20241014123047.png#invert_B]]

Data Integration Architecture focuses on how data flows across different databases and applications, facilitating data movement and transformation. Key components include:

- **Flow of Data:** Examines how data traverses through systems such as Online Transaction Processing (OLTP), Master Data Management (MDM), Data Warehousing (DW), and Business Intelligence (BI).
  
- **The Corporate Information Factory:** A conceptual framework for organizing and managing enterprise data.

- **Master Data Management Hubs:** Central repositories for managing critical data entities.

- **Operational Data Stores (ODS):** Databases that integrate data from various sources for operational reporting and analysis.

- **Data Warehouses and Data Marts:** Systems designed to store and analyze large volumes of historical data.

- **Data Replication and Transformation:** Processes that ensure data consistency and quality across systems.

- **Subscribe and Publish Model:** A pattern for distributing data updates among applications.

- **Batch vs. Near-Real-Time:** Considerations for how frequently data is updated, with technologies like asynchronous message queues for real-time data handling.

- **XML, Web Services, and SOA:** Standards and technologies that facilitate data exchange and integration.

- **“Replacing Feeds with Reads”:** A paradigm shift towards accessing data on-demand instead of relying on periodic data feeds.

## Database Architecture

Database Architecture involves selecting and implementing the appropriate database management systems (DBMS) and integration tools. Key considerations include:

- **Selection of DBMS Tools:** Evaluating and choosing the right DBMS for specific use cases.
  
- **Integration Tools:** Identifying tools that facilitate data integration across systems.

- **Technology Application:** Determining when and where to apply specific technologies for optimal performance.

- **Distribution vs. Federation:** Understanding when to distribute data across systems versus federating access to centralized data sources.

## Unstructured Information Architecture

Unstructured Information Architecture addresses the management of non-relational data types. Essential components include:

- **Enterprise Content Management:** Systems for managing unstructured information throughout its lifecycle.

- **Enterprise Taxonomies:** Structured frameworks for organizing and categorizing information.

- **Enterprise Portal Strategy:** A strategy for providing access to information and applications through a unified platform.

- **Document Management and Imaging Systems:** Tools for managing documents, images, and other media.

- **Storage Management/Archival and Retrieval:** Solutions for efficiently storing and retrieving unstructured data.

- **Report Format, Storage, and Distribution:** Standards and practices for creating, storing, and disseminating reports.

## Essential Elements for Data Alignment and Integration

For successful data alignment and integration, organizations must focus on:

- **Consistent Data Definitions:** Establishing a common understanding of data across the organization.
  
- **Data Quality Management:** Ensuring data is accurate, complete, and timely.

- **Interoperability:** Enabling different systems and applications to work together seamlessly.

- **Data Governance:** Implementing policies and procedures for data management and accountability.

## Metadata Architecture

> Metadata Architecture
> ![[Pasted image 20241014122833.png#invert_B]]

Metadata Architecture provides a structured approach to managing metadata, which describes the context, content, and structure of data. Key elements include:

- **Managed Metadata Environment (MME) Architecture:** A framework that encompasses the hardware, software, staff, and processes dedicated to metadata management.

- **Integration, Control, and Delivery of Metadata:** Ensuring that metadata is effectively managed and accessible.

- **Easier Access to Integrated Metadata:** Streamlining the retrieval of metadata to support decision-making and data management processes.

- **Centralized, Hierarchical, Distributed, or Federated:** Deciding on the organizational structure of metadata management to best fit the needs of the organization.