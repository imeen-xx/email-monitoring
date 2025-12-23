# Sell-out Email Monitoring

This project provides a **Power BI dashboard** designed to monitor sell-out data collection through email interactions.  
It transforms unstructured email exchanges into structured indicators that support process understanding and operational control.

***

## Project Scope

*   Monitoring email-based data collection
*   Measuring data delivery reliability
*   Quantifying follow-up effort
*   Providing visibility on communication complexity

***

## Key Indicators

*   **Reliability** – consistency of data delivery relative to follow-up effort
*   **Files Received** – emails containing sell-out data
*   **Follow-ups Sent** – reminders sent
*   **Total Conversations** – overall interaction volume

Reliability is classified into **High**, **Medium**, and **Low** states.

***
### Project Structure

**Data Model**  
The report is built on a single table (`Email`), intentionally kept flat to reflect the event-based nature of email communications.  
The model is designed for operational monitoring rather than relational analysis.

**Measures Architecture**  
All business logic is implemented through DAX measures, structured in layers:
- Base measures capturing follow-up activity and received files  
- Role-specific measures focusing on operational senders  
- A synthesized KPI measuring data delivery reliability relative to follow-up effort  

This approach keeps the data model simple while embedding business rules directly in the metric layer.

**Report Design Logic**  
The dashboard consists of a single page, designed as a monitoring view rather than an exploratory report.  
The layout prioritizes clarity, fast readability, and immediate interpretation of operational status.


***

## Screenshots

The repository includes three screenshots illustrating:

*   High reliability scenarios
*   Medium reliability scenarios
*   Low reliability scenarios

***

## Dataset

The dataset included in this repository is **synthetic** and created solely for demonstration purposes.

***

## Tools

*   Power BI
*   Excel

*** 
## Link 
https://app.powerbi.com/groups/me/reports/febcf43c-5ec0-4d94-899c-0d2f3e88754a/f5d8e4ea0eafb2e62ab4?experience=power-bi


