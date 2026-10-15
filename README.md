# 🏦 Bank Loan Analysis - Interactive Power BI Dashboard

## 🚀 Project Overview
This project is an end-to-end, interactive Bank Loan Analysis Dashboard developed in Microsoft Power BI. Using a comprehensive financial dataset, this dashboard transforms raw loan data into actionable insights for financial institutions. It empowers stakeholders to evaluate lending performance, monitor high-risk (Bad) vs. low-risk (Good) loans, and analyze borrower demographics, loan purposes, and regional trends through dynamic visual storytelling.

## 🛠 Technical Challenges & Solutions
During the data modeling and dashboard development phase, several technical challenges were resolved to ensure 100% data accuracy and a clean user interface:

1. **Resolving Capacity/License Errors in Visuals:**
   * **Problem:** Plotting large currency figures and high-precision decimals in Matrix and Card visuals resulted in an 'X' icon and a "capacity or license issue" error.
   * **Solution:** Explicitly formatted the DAX Measures (`Total Funded Amount`, `Total Amount Received` as Currency `$`, and `Avg Interest Rate`, `Avg DTI` as Percentage `%`) from the Measure Tools tab, allowing Power BI to render large values accurately.

2. **Dynamic Visual Filtering & Blank Axis Issues:**
   * **Problem:** The Loan Purpose Bar Chart displayed a single bar or a completely blank axis when fields were updated during active cross-filtering.
   * **Solution:** Cleared conflicting hidden slicer selections (e.g., "Debt consolidation") and remapped the `purpose` field to the Y-axis to restore full dynamic responsiveness across all categories.

3. **Optimizing Dashboard Layout for PDF Export:**
   * **Problem:** Exporting the dashboard to PDF caused unwanted white margins and distorted chart scaling.
   * **Solution:** Configured the Canvas Settings to a Custom 16:9 pixel ratio and matched the page wallpaper color to the dark blue background theme, resulting in a seamless, margin-free static PDF export.

## 📈 Dashboard Pages & Visual Breakdown
This interactive report contains two main pages, featuring KPI Cards, Core Analytical Visuals, and Dynamic Slicers:

**Page 1: Summary Dashboard**
1. **Executive KPI Cards:** Displays top-level metrics at a glance — Total Loan Applications (39K), Total Funded Amount, Total Amount Received, Avg Interest Rate, and Avg DTI.
2. **Good vs. Bad Loan Issuance (Donut Charts):** Compares low-risk loans (Fully Paid/Current) against high-risk defaults (Charged Off) based on total applications, funded amounts, and received amounts.
3. **Loan Status Grid View (Matrix):** A detailed tabular breakdown of all key metrics categorized by the overarching Loan Status.

**Page 2: Overview Dashboard**
4. **Monthly Loan Trends (Area Chart):** Tracks the volume of loan applications chronologically by Issue Date.
5. **Regional Overview (Filled Map):** Geographic distribution of loan applications across different states.
6. **Loan Term Breakdown (Donut Chart):** Analyzes borrower preference between 36-month and 60-month loan terms.
7. **Employee Length Analysis (Bar Chart):** Shows the relationship between borrower employment experience (e.g., 10+ years) and loan applications.
8. **Loan Purpose (Bar Chart):** Breakdown of primary reasons for taking loans (e.g., Debt Consolidation, Credit Card).
9. **Home Ownership Status (Pie Chart):** Distribution of applicants who Rent, Own, or have a Mortgage.

## 📁 Repository Contents
* `Bank Loan Analysis.pbix` : The fully functional Power BI dashboard containing the data model, DAX measures, and interactive visuals.
* `financial_loan.csv` / `.xlsx` : The raw datasets used for this analysis.
* `BANK LOAN REPORT.png` : A high-resolution image preview of the completed dashboard.
* `BANK LOAN REPORT.pdf` : A static PDF export of the complete dashboard for quick review.
* `Bank Loan PPT Power BI.pptx` : Presentation slides detailing the project structure.
* `Domain Knowledge Doc.docx` / `Query Doc.docx` / `Terminologies in Data.docx` : Supporting documentation outlining financial terminology and SQL queries.

---

## 👨‍💻 Author

**Bayzid Mostak**<br>
*Data Analyst & Visualization Expert*

*   **[LinkedIn]** https://www.linkedin.com/in/bayzid-mostak-data-analyst/
*   **[GitHub]** https://github.com/TusharAlBayzid
*   **Note:** Download the `.pbix` file and open it in Power BI Desktop to experience the fully interactive cross-filtering capabilities of this dashboard.
