# Data Cleaning and Normalization

## Objective
The goal of this task is to clean, normalize, and match company names from the provided dataset to identify and group similar names.

## Files in the Repository

- `data.csv`: The core dataset containing the company names.
- `normalize_company_names.py`: The Python script used for cleaning, normalizing, and matching company names.
- `cleaned_company_data.csv`: The resulting dataset after all transformations.

## Steps Performed

1. **Load Dataset**:
   - Loaded the provided dataset using Python.

2. **Normalize and Clean Company Names**:
   - Standardized known variations of company names using a predefined dictionary.

3. **Standardize Variations**:
   - For example, "Microsoft Corporation" and "Microsoft Corp" were standardized to "microsoft".

4. **Group Similar Names**:
   - Used a matching technique to identify and group similar company names.
   - Set a minimum threshold score to get the needed results.

5. **Assign Unique IDs**:
   - Assigned a unique ID to each group of similar names.

6. **Map Original Names to Group IDs**:
   - Ensured each original company name mapped to its group representative and group ID.

7. **Documented Logic and Methods**:
   - Documented the logic and methods used for cleaning, normalizing, and matching company names.


## Code Explanation

The Python script `normalize_company_names.py` contains detailed comments explaining each step of the transformation process.

## Results
The final transformed dataset is saved as cleaned_company_data.csv and includes all the applied transformations according to the criteria specified.

## Challenges
Achieving precise matches using the Fuzzywuzzy algorithm, balancing between sensitivity and avoiding excessive false positives.
Opting to use a dictionary to map standardized names instead.

