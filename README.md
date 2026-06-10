# Subdivision Development Lifecycle Analytics and Workflow Automation for Water Utilities

## Executive Summary

Using Python, Excel, ArcGIS Online, and ArcGIS Dashboards, I developed an automated solution to monitor and report on subdivision development activity across the utility's service area. The solution consolidated multiple subdivision checklist workbooks into a single standardized dataset, normalized inconsistent naming conventions, applied management-defined business rules to determine subdivision phase status, and synchronized updates to GIS. Automated workflows maintained the connection between operational checklists and geospatial records through the use of persistent unique identifiers. The resulting dashboard provided leadership with visibility into subdivision progress, development pipelines, and workload distributions while reducing the manual effort required to compile and maintain reports.

---

## Dashboard Overview

![Dashboard Overview](images/Subdivision Development Lifecycle Analytics and Workflow Automation for Water Utilities-Dashboard Home Page.png)

---

## Business Problem

Subdivision development information was maintained across numerous Excel checklists with inconsistent naming conventions and no centralized method for tracking project status. Leadership lacked visibility into how many subdivisions were progressing through each stage of development and relied on manually compiled reports to understand development activity. In addition, repeated updates to subdivision checklists created challenges in maintaining continuity between operational records and GIS features. A solution was needed to consolidate disparate data sources, standardize reporting, automate status calculations, and provide stakeholders with a reliable view of the subdivision development pipeline.

---

## Methodology

1.	Developed a Python workflow to extract subdivision checklist information from multiple Excel workbooks stored within a shared folder.
2.	Standardized inconsistent naming conventions using a field mapping workbook maintained outside the codebase to support ongoing updates without modifying scripts.
3.	Consolidated all subdivision records into a single master Excel dataset representing the authoritative source of operational information.
4.	Implemented management-defined business rules to automatically determine subdivision phase status based on completed and pending checklist items.
5.	Stored phase logic externally within an Excel logic table to improve maintainability and allow future adjustments without altering the automation scripts.
6.	Generated and maintained persistent unique subdivision identifiers to ensure updates consistently referenced the correct GIS features over time.
7.	Geocoded subdivision locations using checklist location information to support spatial reporting and visualization.
8.	Developed a second Python workflow that synchronized cleaned records, calculated phase statuses, and related attributes to ArcGIS Online feature layers.
9.	Automated both workflows using scheduled processes so that source data consolidation occurred first, followed by GIS synchronization and reporting updates.
10.	Designed custom Arcade expressions to replicate the appearance and functionality of management's existing Excel checklists within ArcGIS Online pop-ups.


---

## Skills

Python
•	ETL Development
•	Workflow Automation
•	Business Rules Implementation
•	Data Standardization
•	Master Data Consolidation
•	Scheduled Processing
Excel
•	Data Integration
•	Field Mapping
•	Logic Tables
•	Checklist Management
•	Data Validation
•	Reference Tables
GIS
•	ArcGIS Online
•	Feature Services
•	Address Geocoding
•	Spatial Reporting
•	Arcade Expressions
•	Custom Pop-up Design
Data Visualization
•	ArcGIS Dashboards
•	KPI Development
•	Interactive Filtering
•	Status Reporting
•	Pipeline Monitoring
Analytical Techniques
•	Development Lifecycle Analysis
•	Workflow Automation
•	Phase Classification
•	Master Data Management
•	Operational Reporting


---

## Results & Business Recommendations

The automated solution transformed disconnected subdivision checklists into a centralized operational intelligence platform capable of tracking subdivision activity from initiation through completion. By standardizing data sources, automating phase calculations, and synchronizing updates to GIS, leadership gained visibility into the overall development pipeline without relying on manually compiled reports.
The dashboard provided real-time metrics illustrating how many subdivisions existed within each development phase while displaying color-coded subdivision locations throughout the service area. Persistent subdivision identifiers ensured that repeated checklist updates continued to reference the same GIS records, preserving historical continuity and preventing duplicate reporting. The custom Arcade pop-ups further enhanced usability by presenting subdivision information in a format familiar to management, reducing the learning curve associated with transitioning from spreadsheets to GIS.
Based on these findings, the following recommendations were developed:
1.	Continue utilizing automated phase calculations to ensure consistent subdivision status reporting across departments.
2.	Use dashboard metrics to identify bottlenecks within the subdivision development lifecycle and prioritize follow-up activities.
3.	Maintain externally managed field mappings and business logic tables to simplify future process modifications without requiring code changes.
4.	Expand the use of persistent identifiers across additional operational processes to improve data governance and reporting consistency.
5.	Leverage GIS-based reporting as the primary source of subdivision status information to reduce reliance on manually compiled spreadsheets.


---

