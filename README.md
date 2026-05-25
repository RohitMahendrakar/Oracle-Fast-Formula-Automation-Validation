# Oracle Fusion HCM Fast Formula – Payroll & Absence Management

## 📌 Project Overview

This project demonstrates the implementation of multiple Oracle Fusion HCM Fast Formula scenarios across Payroll and Absence Management modules. The project includes custom Fast Formula development, eligibility profile validations, accrual calculations, payroll calculations, person selection logic, DFF usage, and custom lookup integrations.

The implementation focuses on real-time business scenarios using Oracle Fusion HCM Fast Formula syntax, database items, contexts, defaults, input statements, conditional logic, and formula return structures.

The repository also contains screenshots related to all implemented scenarios, configurations, and testing activities for better understanding of the setup and execution process.

---

# 🚀 Modules Covered

- Oracle Payroll
- Oracle Absence Management
- Eligibility Profiles
- Global Absence Accrual Plans
- Payroll Elements
- Person Selection Formulas
- DFF (Descriptive Flexfields)
- Custom Lookups
- Validation Formulas
- Payroll Calculation Formulas

---

# 🧠 Key Concepts Implemented

## ✅ Fast Formula Components

- DEFAULT Statements
- INPUTS ARE Statements
- Local Variables
- Global Variables
- Database Items
- Formula Contexts
- Conditional Logic
- Nested IF Statements
- RETURN Statements
- Date Functions
- Numeric Functions
- Text Functions
- WAS DEFAULTED Conditions
- Formula Compilation & Validation

---

# 🔹 Payroll Formula Scenarios

## 🏠 Housing Allowance Formula

Implemented a Payroll Fast Formula to calculate Housing Allowance dynamically based on Basic Salary.

### 🔸 Features Implemented

- Uses Payroll Database Items
- Handles Employee Termination Conditions
- Uses Payroll Period Dates
- Dynamic Housing Allowance Calculation
- Default Value Handling
- Formula Return Logic
- Local Variable Initialization

### 🔸 Logic Used

```text
Housing Allowance = 25% of Basic Salary
```

### 🔸 Components Used

- `DEFAULT FOR`
- `INPUTS ARE`
- `PAY_EARN_PERIOD_START`
- `PAY_EARN_PERIOD_END`
- `PAY_ASG_TERMINATION_DATE`
- `WAS DEFAULTED`
- Date Functions
- Numeric Calculations

### 🔸 Formula Highlights

- Calculated allowance based on payroll period
- Managed termination scenarios using effective dates
- Used payroll database items and element entry values
- Implemented local variables for optimized calculations

---

# 🔹 Absence Management Scenarios

## 📅 Annual Leave Eligibility Formula

Created Eligibility Profile Fast Formula for Annual Leave eligibility based on Employee Category and Person Type.

### 🔸 Eligibility Conditions Covered

- Permanent Employees
- Consultants
- Trainees
- Staff Employees
- White Collar Employees
- Technical Employees
- Blue Collar Employees
- Civil Servants

### 🔸 Features Implemented

- Employee Category Validation
- Person Type Validation
- Eligibility Flag Handling
- Conditional Logic Processing
- Return Value Configuration

### 🔸 Return Values

```text
Y = Eligible
N = Not Eligible
```

---

# 📊 Global Absence Accrual Formula

Implemented Global Absence Accrual Fast Formula using:

- Length of Service
- Plan Enrollment
- Vesting Logic
- Carryover Rules
- Ceiling Rules
- Proration Factors

### 🔸 Features Implemented

- Dynamic Accrual Calculation
- Service-Based Entitlement Logic
- Carryover Processing
- Ceiling Validation
- Vesting Unit Calculation
- Proration Handling

### 🔸 Business Logic

| Length of Service | Accrual | Ceiling | Carryover |
|------------------|----------|----------|------------|
| Less than 3 Years | 24 Days | 100 | 50 |
| 3 to 5 Years | 30 Days | 120 | 60 |
| Greater than 5 Years | 40 Days | 150 | 75 |

### 🔸 Formula Components Used

- `GET_CONTEXT(EFFECTIVE_DATE)`
- `DAYS_BETWEEN`
- Date Arithmetic
- Nested IF Conditions
- Accrual Variables
- Vesting Units
- Carryover Proration
- Ceiling Proration

---

# 🔹 Person Selection Formula

Implemented custom Person Selection Formula using:

- Employee Numbers
- Assignment-Based Filtering
- Selection Criteria Validation
- Conditional Assignment Logic

### 🔸 Features Implemented

- Employee Filtering
- Assignment Set Processing
- Selection Rule Validation
- Conditional Inclusion Logic

---

# 🔹 DFF (Descriptive Flexfields)

Configured and validated custom DFFs for additional business requirements.

## 🔸 Areas Covered

- Segment Configuration
- Context Sensitive DFF
- Value Set Configuration
- Validation Rules
- DFF Integration with Fast Formula
- DFF-Based Business Logic

---

# 🔹 Custom Lookups

Implemented custom lookups for dynamic validations and business logic processing.

## 🔸 Lookup Usage

- Validation Logic
- Eligibility Mapping
- Dynamic Condition Handling
- Lookup-Based Formula Processing
- Value Retrieval in Formulas

---

# ⚙️ Oracle Fast Formula Concepts Used

## 🔸 Database Items Used

```text
PER_ASG_EMPLOYEE_CATEGORY_MEANING
PER_ASG_USER_PERSON_TYPE
PAY_EARN_PERIOD_START
PAY_EARN_PERIOD_END
PAY_ASG_TERMINATION_DATE
PER_ASG_REL_ORIGINAL_DATE_OF_HIRE
ANC_ABS_PLN_NAME
ANC_ABS_PLN_PLAN_UOM
```

---

## 🔸 Formula Contexts Used

```text
GET_CONTEXT(EFFECTIVE_DATE)
```

---

# 🔹 Formula Types Implemented

| Formula Type | Purpose |
|---|---|
| Oracle Payroll | Payroll Calculations |
| Global Absence Accrual | Leave Accrual Processing |
| Eligibility Profile | Eligibility Determination |
| Person Selection | Assignment Filtering |
| Validation Formula | Input Validation |

---

# 🛠️ Tools & Technologies

- Oracle Fusion HCM
- Oracle Fast Formula
- Oracle Payroll
- Oracle Absence Management
- DFF Configuration
- Custom Lookups
- Oracle HCM Cloud

---

# 📘 Learning Outcomes

Through this project, the following concepts were implemented and understood:

- Oracle Fast Formula Syntax
- Formula Structure and Standards
- Payroll Formula Processing
- Absence Accrual Calculations
- Eligibility Profile Logic
- Database Item Usage
- Formula Context Usage
- Formula Validation Techniques
- DFF Integration
- Lookup Integration
- Formula Optimization Techniques
- Payroll Element Processing
- Formula Compilation & Debugging

---

# 📷 Project Artifacts

The repository contains:

- Formula Screenshots
- Configuration Screenshots
- Payroll Formula Scenarios
- Absence Formula Scenarios
- TXT-Based Formula Files
- Excel Scenario Sheets
- Oracle Fast Formula Reference Documents
- Testing and Validation Screenshots

---

# 🧪 Testing Performed

- Payroll Run Validation
- Formula Compilation Validation
- Absence Accrual Testing
- Eligibility Validation Testing
- Lookup Validation Testing
- DFF Validation Testing
- Formula Return Validation
- Edge Case Testing

---

# 📚 References

- Oracle Fast Formula User Guide
- Oracle Fusion HCM Documentation
- Payroll Fast Formula Scenarios
- Absence Management Formula Scenarios

---

# 👨‍💻 Author

Developed as part of Oracle Fusion HCM technical learning and implementation practice focusing on Payroll and Absence Management Fast Formula scenarios including Payroll Calculations, Eligibility Profiles, Accrual Formulas, DFF Configurations, and Custom Lookup Implementations.
