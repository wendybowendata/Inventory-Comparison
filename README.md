# Inventory-Comparison
Project Title:Inventory Comparison
Objective: To compare two datasets containing pharmacy inventory and pricing
information, identifying discrepancies, analyzing variations in medication prices, and
assessing changes in product availability over time or between different locations. 
Datasets (Simulated):
1. Dataset 1 (e.g., "Pharmacy_Inventory_A"):
1. Medication_ID (Primary Key)
1. Medication_Name
1. Strength
1. Dosage_Form
1. Manufacturer
1. Quantity_On_Hand
1. Unit_Price
2. Dataset 2 (e.g., "Pharmacy_Inventory_B"):
1. Medication_ID (Primary Key)
1. Medication_Name
1. Strength
1. Dosage_Form
1. Manufacturer
1. Quantity_On_Hand
1. Unit_Price

Project Steps:
1. Identify Missing Medications:
Goal: Find medications present in Dataset A but not in Dataset B, and vice
versa.
SQL: Use LEFT JOIN or EXCEPT to find records in one table not present in
the other.

2. Compare Unit Prices:
Goal: Identify medications with different unit prices between the two
datasets.
SQL: Use INNER JOIN to match records and then filter based on
unequal UnitPrice.

3. Analyze Quantity on Hand Differences:
Goal: Determine which medications have different quantities available in
the two datasets.
SQL: Similar to price comparison, use INNER JOIN and filter by
unequal QuantityOnHand.

4. Identify Identical Records:
Goal: Find medications with the same details in both datasets.
SQL: Use INNER JOIN and filter where all relevant columns are equal.

Extensions (for a more advanced project):
1. Handle Data Inconsistencies: Use FULL OUTER JOIN to find rows that exist only in
one table and fill in NULL values where no match exists, useful for identifying
orphaned records or data inconsistencies.
2. Summarize Differences: Aggregate the results to show counts of missing
medications, average price differences, etc.
3. Visualize the Data: Use data visualization tools (e.g., Tableau, Power BI, Python
libraries) to present the comparison results visually.
4. Create a Reusable Function: Encapsulate the comparison logic into a SQL
function for easier reuse.
