# 🏏 IPL Data Cleaning using Pandas 📊

This project focuses on cleaning and processing IPL (Indian Premier League) cricket match data using Python and Pandas. It involves working with two raw CSV files — one containing match-level data and the other containing ball-by-ball delivery-level data — and generating a cleaned, consistent dataset ready for analysis and visualization.

---

## 📦 Project Structure

```
├── IPL_Data_Cleaning.ipynb      # Jupyter Notebook with data cleaning code
├── matches.csv                  # Raw match-level dataset
├── deliveries.csv               # Raw delivery-level dataset
├── cleaned_data.csv             # Final cleaned and processed dataset
└── README.md                    # Project description and details
```

---

## 📊 Data Files

- **`matches.csv`** → Contains details of IPL matches from 2008 to 2024 (match IDs, teams, venues, results, etc.)
- **`deliveries.csv`** → Ball-by-ball delivery details for all matches (runs, extras, dismissals, etc.)
- **`cleaned_data.csv`** → Final cleaned dataset after merging, filling missing values, correcting team and venue names, and handling inconsistencies.

---

## 🔧 Features of the Cleaning Process

- Removed duplicate venue and team names, standardized naming conventions
- Handled missing values in critical columns like:
  - `city` (filled based on venue)
  - `result_margin`, `target_runs`, `target_overs` (logical fills based on match conditions)
  - `method` (set based on target overs and D/L method usage)
- Merged match-level and delivery-level data cleanly
- Fixed result inconsistencies (e.g. matches marked as 'tie' having a winner)
- Generated a consistent and clean final dataset for analysis

---

## 📓 Tools & Libraries

- **Python 3.x**
- **Pandas**
- **NumPy**
- **Jupyter Notebook**

---

## 📈 How to Run

1. Clone the repository
2. Install required libraries:
   ```
   pip install pandas numpy jupyter
   ```
3. Open `IPL_Data_Cleaning.ipynb` in Jupyter Notebook
4. Run the cells to see the cleaning process step-by-step
5. The final cleaned data will be saved as `cleaned_data.csv`

---

## 📌 Author

**Rahul MC**  
[GitHub](https://github.com/RAHULMAC05)

---

## 📜 License

This project is open-source and available for public use and modification.
