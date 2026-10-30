Day 4 — AI-Assisted Data Cleaning

Date: October 30, 2026

🎯 Learning Objective

Learn how to identify and handle common data quality issues in Excel using AI-assisted guidance and data-cleaning techniques.

📊 Practice Dataset

Customer

City

Sales

Ravi Kumar

BENGALURU

5,000

Priya Sharma

bengaluru

7,000

Amit Verma

HYDERABAD

4,500

Ravi Kumar

BENGALURU

5,000

Sneha Reddy

CHENNAI

6,000

Rahul Mehta

HYDERABAD



Anjali Rao

CHENNAI

8,000

🧠 What I Practiced

1. Identifying Inconsistent Text

Identified inconsistent city names, such as:

BENGALURU

bengaluru

Practiced using Excel's TRIM and PROPER functions to standardize text.

2. Identifying Duplicate Records

Identified a potential duplicate record for Ravi Kumar.

Used Excel's COUNTIFS function to check for repeated combinations of Customer, City, and Sales.

=COUNTIFS($A$2:$A$8,A2,$B$2:$B$8,B2,$C$2:$C$8,C2)>1

Learning: Identical records may indicate duplicates, but they should be verified before removal.

3. Identifying Missing Values

Identified a missing Sales value for Rahul Mehta.

Learning: A blank value represents missing information and should not automatically be replaced with zero.

💡 Data Cleaning Decisions

Issue

Decision

Inconsistent city names

Standardized using Excel functions

Potential duplicate record

Identified; imagined removal for practice

Missing Sales value

Kept blank pending confirmation

🤖 How I Used AI

I used ChatGPT inside Excel to:

Understand common data quality issues.

Learn how to identify duplicates and missing values.

Practice data-cleaning techniques.

Understand how to standardize inconsistent text.

Review decisions before modifying the data.

📚 Key Takeaways

Data cleaning is an essential step before analysis.

Inconsistent text can affect grouping and reporting.

Duplicate records should be verified before deletion.

Missing values should not automatically be treated as zero.

AI can guide data cleaning, but the analyst must validate the data and decisions.

📝 Reflection

Today I practiced identifying and handling common data quality issues using Excel and AI-assisted guidance.

I learned that data cleaning is not just about applying formulas—it also requires careful judgment and verification.

In real-world scenarios, I would confirm duplicate records and missing values with the appropriate source before making changes.

Day 4 completed! 🚀
