# 🚗 SAP Sales & Distribution Portal – SmartSale Ltd.

This project is a custom SAP Sales & Distribution (SD) application developed using **ABAP Module Pool Programming**. Designed for SmartSale Ltd., an automobile manufacturing company, the solution automates key sales processes such as customer registration, inquiry handling, quotation generation, and order completion within the SAP ERP system.

---

Project Video Demonstration link [https://drive.google.com/file/d/1TBfaOvHE2361G4mgVM2rsG-GagKK1Rz0/view?usp=sharing]

## 📌 Features

- **Customer Login & Registration**
  - Secure login with auto-generated Customer ID.
  - Profile update functionality (Screen 500) for name, password, and security question.

- **Customer Dashboard**
  - ALV Grid showing open orders with selection capability.
  - Buttons to create inquiry, request follow-up, cancel order, or respond to quotations.
  - Email notifications triggered via **CL_BCS**.

- **Admin Dashboard**
  - Order status filter (Open, Cancelled, Completed).
  - Popup-based quotation creation with dynamic pricing and stock checks.
  - Fulfillment logic and invoice generation using **Smartforms**.

- **Smartforms & Workflows**
  - Automated quotation and invoice PDF generation.
  - Real-time email communication on inquiry, approval, and rejection events.

---

## 📂 Custom Tables Used

| Table Name            | Description                                  |
|-----------------------|----------------------------------------------|
| `ZCUSTOMER_DETAILS`   | Stores customer registration & profile data  |
| `ZMATERIAL_MASTER`    | Product and inventory information            |
| `ZINQUIRY_HEAD/ITEM`  | Header & item-level inquiry data             |
| `ZQUOTATION_HEAD/ITEM`| Header & item-level quotation data           |
| `ZORDER_STATUS_LOG`   | Tracks order status changes and history      |

---

## ⚙️ Technologies & Tools

- **ABAP Module Pool Programming (SE80, SE51, SE41)**
- **SAP Data Dictionary (SE11)**
- **ALV Grid Display**
- **BDC for Data Upload**
- **SAP Smartforms**
- **CL_BCS for Email**
- **SAP Workflows (SWDD)**

---

## 🧪 Testing & Validation

- All screens and workflows tested with sample data.
- ALV selection logic and screen validations verified.
- Smartforms and email triggers confirmed for all major events.

---

## 📈 Future Enhancements

- SAP Fiori/UI5-based front-end for mobile access.
- Role-based authorization using SAP auth objects.
- Reporting and analytics dashboard integration.
- Push notification support via third-party API.

---

## 📁 Project Structure

/module_pool_project/
│
├── Screens/
│   ├── Login (100)
│   ├── Registration (200)
│   ├── Customer Dashboard (300)
│   ├── Admin Dashboard (400)
│   └── Profile Update (500)
│
├── Includes/
│   ├── PBO_PAI logic
│   ├── Validations
│   └── Database operations
│
├── Forms/
│   ├── Quotation Smartform
│   └── Invoice Smartform
│
└── Documentation/
    └── Project Report, PPT, Screenshots


