# Spotify + YouTube Music – Data Cleaning & Preparation
 # Project Overview
This project involved the cleaning, validation, and preparation of a combined dataset from Spotify and YouTube Music to support accurate analysis and visualization in Power BI. The goal was to transform raw, unstructured, and incomplete data into a reliable, analysis-ready dataset while preserving data integrity and real-world context.

# Objectives
Identify and responsibly handle missing and invalid data

Fix merged columns and poor structural formats

Standardize naming conventions and enforce correct data types

Remove irrelevant or non-analytical columns

Validate duplicates without unnecessary data loss

Prepare a clean dataset optimized for Power BI reporting and dashboards

# Dataset Description
The dataset includes music track information from both platforms, containing:

 Artist and track metadata

 Album details

 Engagement metrics (views, likes, comments, streams)

 Audio features (danceability, energy, tempo, etc.)

 Platform and licensing attributes

 Tools & Technologies Used
Power BI Desktop

Power Query (M Language) for data transformations

CSV as the raw data source

# Data Cleaning & Preparation Steps
1. Handling Missing Values
Removed rows with missing license data where most attributes were absent

Imputed missing engagement metrics (views, likes, etc.) using artist-level averages instead of global means

2. Fixing Merged Columns
Split merged Spotify columns using | delimiter

Split merged YouTube columns using - delimiter

Retained only relevant fields for analysis

3. Standardizing Naming Conventions
Converted all column names to lowercase

Removed redundant prefixes/suffixes from artist and track columns

4. Removing Irrelevant Columns
Dropped non-analytical columns: random_1, random_2, unnamed, URL fields, and platform-specific IDs

5. Correcting Data Types
Enforced proper data types: numeric, text, and boolean

Resolved inconsistencies in columns like danceability

6. Handling Invalid Data Entries
Converted invalid numeric entries in views to null, then imputed using artist averages

Preserved descriptive metadata (e.g., numeric-like album names stored as text)

7. Duplicate Validation
Verified that repeated track names belonged to different artists or channels

No true duplicates were removed

8. Reordering & Renaming Columns
Organized columns into logical groups: identification, audio features, engagement metrics

Renamed columns for clarity (e.g., view → views)

✅ Final Outcome
✅ Clean, consistent, and analysis-ready dataset

✅ No meaningful data loss

✅ Context-aware imputation preserves real-world patterns

✅ Optimized for Power BI visualization and reporting

# Project Files
Spotify YouTube Music Data Cleaning Report.pdf – Detailed step-by-step documentation

Raw Dataset Link - https://drive.google.com/file/d/1qanyuwEzkwEJ73vDJHk4ZIWE0JUG7udb/view

Cleaned_file.pbix – Power BI file with applied transformations

README.md – Project overview and methodology
