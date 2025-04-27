1. Data Cleaning & Redundant Column Removal
Removal of Standard Deviation Columns: All columns starting with sd_ were dropped to retain only mean values of environmental metrics.
Elimination of Redundant Columns: The grouping column was removed, as its information was fully represented by diet_group, sex, and age_group.
2. Data Aggregation & Batch Merging
Consolidation of Monte Carlo Batches: Data was grouped by diet type (diet_group), gender (sex), and age group (age_group) to merge results across multiple Monte Carlo simulation batches (mc_run_id):
Environmental Metrics: Calculated the mean across simulation batches.
Participant Count: Summed across batches to reflect total sample size.
3. Column Renaming & Readability Enhancement
Descriptive Renaming: Technical column names were replaced with intuitive labels.
Diet Type Label Standardization: Abbreviated categories were mapped to human-readable names.
