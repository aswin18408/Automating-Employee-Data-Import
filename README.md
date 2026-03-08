# Automating-Employee-Data-Import
ServiceNow project for automating employee data import using Import Sets, Dot Walking and Dictionary Override.
Automating Employee Data Import
Project Overview

The Automating Employee Data Import project is developed to automate the process of importing employee data into the system and improve incident management efficiency. This project demonstrates how automation techniques can be used to reduce manual work and ensure accurate data management.

The project is implemented using the ServiceNow platform. It uses important features such as Import Sets, Transform Maps, Dot Walking, and Dictionary Override to automate data handling and improve the incident resolution process.

This system allows organizations to import employee details from an external file and automatically display relevant employee information when incidents are assigned.

Problem Statement

Organizations often receive employee data from external systems such as spreadsheets or HR platforms. Manually entering employee records into the system takes time and may lead to errors.

When incidents are assigned to employees, incident handlers need quick access to employee details like department and manager email. Without automation, users must search multiple records to find this information.

Additionally, incidents often require a different priority level compared to other task-related tables. However, the default priority value is inherited from the task table, which may not reflect the urgency of incidents.

Objective

The objective of this project is to automate employee data import and improve incident management efficiency.

The main goals of the project are:

Automate employee data import from external files

Reduce manual data entry

Display employee department and manager details in the incident form

Customize the default priority value for incidents

Improve efficiency in incident management

Technologies Used

This project is developed using the following technologies and concepts:

ServiceNow

Import Sets

Transform Maps

Dot Walking

Dictionary Override

Microsoft Excel / Google Sheets

Project Workflow
1. Employee Data Creation

Employee data is first created in a spreadsheet with the following fields:

Name

Email

Department Manager

Manager Email

The spreadsheet is saved and downloaded as a CSV or Excel file.

2. Import Data Using Import Sets

The employee data file is uploaded into the system using Import Sets.

Steps include:

Navigate to System Import Sets

Select Load Data

Create a new import set table

Upload the employee data file

The imported data is stored temporarily in the import set table.

3. Transform Map

A transform map is created to transfer data from the import set table to the user table.

Configuration includes:

Source Table: Import Employee Data

Target Table: User (sys_user)

The transform map ensures that fields from the imported file are correctly mapped to the system fields.

4. Dot Walking Implementation

Dot walking is used to retrieve related information from reference fields.

In the incident form, the following fields are displayed automatically when an employee is assigned:

Assigned To Department

Assigned To Email

Assigned To Manager

This helps incident handlers quickly access employee information.

5. Dictionary Override

The incident table extends the task table and inherits its fields.

Using dictionary override, the default value of the priority field is customized specifically for the incident table.

The default priority is set to:

3 – Moderate

This ensures that incidents receive appropriate priority values.

Project Features

Automated employee data import

Data mapping using transform maps

Automatic display of employee details in incident forms

Custom priority configuration for incidents

Improved incident management workflow

Project Benefits

Reduces manual data entry

Improves data accuracy

Saves time for administrators

Provides quick access to employee information

Improves incident resolution efficiency 


project demo video link:

https://drive.google.com/file/d/1IXqaupRDyliQq4GVa8t1EAREYM0LnAjt/view?usp=drive_link

TEAM PROJECT:"NAAN MUDHALVAN"

Team ID : SWTID-2026-3553
Team Size : 4
Team Leader : ASWIN MEHARAJ BANU A
Team member : S ASMITHA BANU
Team member : BAGAVATHI I
Team member : BHATHI MUTHU JOHARABEEVI J

Conclusion

The Automating Employee Data Import project successfully demonstrates how automation features in ServiceNow can improve data management and incident handling. By using Import Sets, Dot Walking, and Dictionary Override, the system provides a more efficient way to manage employee data and incident workflows.

This project helps organizations streamline operations, reduce errors, and improve productivity.
