# 📊 SAP-SALES-PURCHASE-ORDER-REPORT

## 🔧 Technology Stack

- SAP ABAP (Advanced Business Application Programming)  
- ALV Grid Reporting  
- Function Modules  
- Custom Tables  
- Module Pool Programming (for selection UI)  
- Selection Screens and Dynamic Filters  

---

## 📘 Project Description

The `SAP-SALES-PURCHASE-ORDER-REPORT` is a custom ABAP report that delivers a consolidated and dynamic view of **Sales Orders** and **Purchase Orders**. Designed for real-time business analysis, it offers a user-friendly **ALV-based interface** for stakeholders to monitor and evaluate transactional data efficiently.

The solution includes **dynamic selection criteria**, **reusable function modules**, and **ALV grid output** for a seamless user experience—all within a single program.

---

## 📋 Key Features

### ✅ Dual Mode Report
- Toggle between **Sales Order Mode** and **Purchase Order Mode** using radio buttons on the selection screen.

### 🧾 Dynamic Selection Criteria
- Filters data using:
  - Date Range  
  - Sales Org / Purchase Org  
  - Customer / Vendor  
  - Material / Plant  
- Built using `SELECT-OPTIONS` and `PARAMETERS`.

  <img width="975" height="475" alt="image" src="https://github.com/user-attachments/assets/9f315b01-fdd4-4667-83da-ce45605559e4" />


### 🛠️ Custom Function Modules
- Reusable FM architecture:
  - `ZFM_GET_SALES_DATA`  
  - `ZFM_GET_PURCHASE_DATA`  
- Fetches enriched master data like vendor/customer names from **LFA1**, **KNA1**, etc.

  <img width="975" height="439" alt="image" src="https://github.com/user-attachments/assets/bc640c28-f76d-475b-b848-204f6102f6e7" />


### 📊 ALV Grid Output
- Interactive ALV display with:
  - Column sorting & filtering  
  - Totals and subtotals  
  - Column resizing  
  - Layout saving
 
<img width="975" height="461" alt="image" src="https://github.com/user-attachments/assets/fcbb5fa6-b71d-43ac-872e-63c791341aaa" />


### 🧾 Field Catalog & Layout Customization
- Enhanced formatting using `LVC_FCAT`:
  - Currency and quantity alignment  
  - Text wrapping & alignment
  



