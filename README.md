📌 Project Title: SAP-SALES-PURCHASE-ORDER-REPORT
🔧 Technology Stack:
SAP ABAP (Advanced Business Application Programming)

ALV Grid Reporting

Function Modules

Custom Tables

Module Pool Programming

Selection Screens and Dynamic Filters

📘 Project Description:
The SAP-SALES-PURCHASE-ORDER-REPORT is a custom-developed ABAP report designed to provide a consolidated view of both Sales Orders and Purchase Orders within the SAP system. It serves as a single, user-friendly interface for business stakeholders to analyze real-time transactional data related to sales and procurement.

This report was built using ALV (ABAP List Viewer) for rich, interactive output and incorporates dynamic filters, custom logic, and modularized code for efficient performance.

📋 Key Features:
✅ Dual Mode Report:

Allows users to switch between Sales Order Report and Purchase Order Report using radio buttons on the selection screen.

🧾 Dynamic Selection Criteria:

Users can filter data by date range, document type, vendor/customer, material number, and plant using SELECT-OPTIONS and PARAMETERS.

🛠️ Custom Function Modules:

Used to fetch vendor and customer names from standard tables like LFA1, KNA1, etc., using modular and reusable code architecture.

📊 ALV Grid Output:

The data is displayed using ALV GRID with features such as column sorting, filtering, totaling, and column resizing for a seamless user experience.

🧾 Field Catalog & Layout Customization:

Enhanced readability using appropriate field catalog settings including currency/quantity alignment, text alignment, and hotspot support.

🔁 Reuse of Structures:

Used custom type definitions (ZTY_SALES_PURCHASE) to hold report data dynamically and uniformly for both order types.

🧩 Technical Implementation:
Selection Screen:

Implemented using SELECTION-SCREEN BEGIN OF BLOCK, PARAMETERS, and SELECT-OPTIONS to support advanced filters.

Example filters: Sales Org, Purchase Org, Material, Plant, Customer, Vendor.

Custom Tables Used (if any):

ZTABLE_ORDER_CONFIG – Holds configurations related to sales/purchase order filters.

Modularization:

Data-fetch logic modularized into:

ZFM_GET_SALES_DATA

ZFM_GET_PURCHASE_DATA

ALV Logic:

Used CL_GUI_ALV_GRID and REUSE_ALV_GRID_DISPLAY depending on output type.

Field catalog built using LVC_FCAT and layout using LVC_S_LAYO.

🧵 Screens & Flow:
Initial Selection Screen with Filters

<img width="975" height="475" alt="image" src="https://github.com/user-attachments/assets/39f4856d-2675-4f05-bdf9-75ae5e55156a" />


Radio buttons for Sales / Purchase Report

Date range, Material, Vendor, etc.

Custom Function Module Fetch Execution

<img width="975" height="439" alt="image" src="https://github.com/user-attachments/assets/a226c2f5-c41d-47ba-83b9-003ca04da885" />


Fetches description for customers, vendors, and materials.


Displaying ALV output SO/PO Number, Vendor Name, Material, Quantity Ordered, Net Price, etc.

<img width="975" height="461" alt="image" src="https://github.com/user-attachments/assets/27a57a83-2689-4410-beb0-d8e8e939771a" />


📈 Business Impact:
Enabled faster analysis of critical sales and procurement data directly in SAP GUI.

Reduced manual effort to gather and filter reports from multiple transactions like VA05, ME2N, etc.

Improved accuracy and decision-making efficiency for procurement and sales departments.

🔒 Authorization & Security:
Implemented authorization checks to restrict access to users with appropriate roles (e.g., Sales Analyst, Purchase Clerk).

Used AUTHORITY-CHECK for authorization object validation.

📅 Planned Enhancements (Future Scope):
Email delivery of ALV reports using SAP BCS (Business Communication Services)

Integration with SAP SmartForms to generate printable PDF reports

Role-based access for selection screen elements
