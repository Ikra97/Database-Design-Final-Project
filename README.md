DMDD Final Project


Project Overview

The purpose of this project is to develop an integrated Hospital Management System to streamline the management of various entities within hospitals. The objective is to create a centralized database to enhance system efficiency by maintaining all the necessary information required to administer hospitals. Additionally, the project includes visualization tools to exhibit and convey data trends for prevalent outbreaks, aiding in better comprehension of analytics based on collected hospital data.

Dataset

Source

The datasets were obtained from multiple sources:

•	https://www.kaggle.com/

•	https://healthdata.gov/

•	https://www.who.int/data


Features

•	Hospital Admin Table: Admin_ID, Admin_Name, Contact_No, Email_ID.

•	Doctor Table: Doc_ID, lst_nm, frst_nm, pri_spec, cty, st, phn_numbr, age.

•	Patient Table: P_ID, F_name, L_name, age, Gender, Phone, Email, B_Grp, Address, State, City, Admit_Date, Discharge_Date.

•	Bill Payment Table: Bill_ID, Bill_Date, P_ID, Doc_Fees, Room_Charge.

•	Record Table: R_ID, Doc_ID, P_ID, Bill_ID.


Preprocessing Steps

•	Hospital Admin Table: Read CSV file, removed null values, and verified data accuracy.

•	Doctor Table: Web scraped data, read CSV file, removed null values, grouped by primary spec and count, plotted bar graphs for primary spec and age.

•	Patient Table: Read CSV file, removed null values, converted Admit_Date to month-year format, grouped data, and generated line graphs.

•	Bill Payment Table: Read CSV file, removed null values, converted Bill_Date to month-year format, and plotted line graphs.

•	Record Table: Read CSV file, removed null values, and verified data accuracy.


Project Structure

•	/data: Contains all the CSV files used for the project.

•	/scripts: Python scripts for web scraping, data cleaning, and preprocessing.

•	/visualizations: Contains the generated graphs and plots.

•	/database: SQL scripts for creating and populating the database tables.

•	README.md: Project documentation.



Methodology

Data Collection

•	Web Scraping: Used Python scripts to scrape doctor data from the Browse AI website.

•	Manual Entry: Input data for hospital admin, patients, bill payments, and records manually.

Data Processing

•	Cleaning: Removed null values using Python and Jupyter.

•	Grouping and Aggregation: Grouped data by relevant columns and calculated aggregates.

•	Visualization: Plotted data using Matplotlib to visualize trends.

Database

•	Creation: Created tables using SQL scripts.

•	Normalization: Normalized data to remove redundancy and improve efficiency.


Views

Created various views to analyze data, such as:

•	bill_date_patients

•	avg_bill_patient

•	doctor_patient_perstate

•	highest_fees

•	highest_patients

•	highest_room_charges

•	highestpay_doctor

•	no_of_patients

•	patient_bill_record

•	patient_doctor_sees

•	patient_treated_speciality

•	patients_admitted

•	room_charges

•	track_doctor

•	no_oftimes_admitted


Results

•	Visualizations demonstrated key trends and patterns in the data, such as the number of patients per month, average room charges per state, and the number of doctors per state.

•	Created views provided insights into the billing dates, average bills, patient-doctor interactions, and more.


Conclusion

The integrated Hospital Management System successfully consolidated hospital data, enhanced management efficiency, and provided valuable insights through data visualization. Future steps could include integrating real-time data updates and expanding the system to include more hospitals.

![image](https://github.com/Ikra97/Database-Design-Final-Project/assets/113316391/14118440-bc67-4c7b-8b8c-91ba032401f4)
