# County Rainfall and Planting Advisory

## 1. Project Summary

This project analyzes monthly rainfall data from five Kenyan counties: Nairobi, Nakuru, Kisumu, Mombasa, and Machakos.

The analysis uses Python and NumPy to clean rainfall data, calculate annual rainfall totals, determine average monthly rainfall, identify the wettest months, count dry months, and recommend planting windows based on consecutive two-month rainfall patterns.

The project also exports the results into a CSV summary file for further analysis.

## 2. Project Objectives

- Clean missing and invalid rainfall records in the Machakos dataset.
- Combine the five counties into a NumPy array.
- Calculate annual rainfall totals for each county.
- Calculate average monthly rainfall across all counties.
- Identify the wettest month for each county.
- Count months receiving less than 50 mm of rainfall.
- Identify the two consecutive months with the highest combined rainfall.
- Export the analysis results into a CSV file.

## 3. Technologies and Libraries

- Python
- NumPy
- CSV (Python standard library)
- Jupyter Notebook

## 4. Project Files

| File | Description |
|---|---|
| `README.md` | Project documentation and instructions |
| `rainfall_analysis.ipynb` | Jupyter Notebook containing data cleaning and analysis |
| `rainfall_summary.csv` | Summary of rainfall results for the five counties |
| `requirements.txt` | Required Python libraries |

## 5. How to Run the Project

1. Clone or download this repository.
2. Open the project directory in Command Prompt.
3. Install the required library:

   `pip install -r requirements.txt`

4. Launch Jupyter Notebook:

   `jupyter notebook`

5. Open `rainfall_analysis.ipynb`.
6. Select **Kernel → Restart Kernel and Run All** to execute the analysis.
7. The notebook generates `rainfall_summary.csv` in the project directory.

## 6. Planting Advisory

- Nairobi, Nakuru, Kisumu, and Mombasa have April–May as their highest consecutive two-month rainfall window.
- Machakos has November–December as its highest consecutive two-month rainfall window and records six dry months.
- Farmers should consider crop requirements, soil conditions, water availability, and seasonal weather forecasts before making planting decisions.

## 7. Data Quality Notes

The original Machakos dataset contained two invalid readings: `N/A` for April and an empty value for September. These were replaced with the rounded average of the ten valid readings, which is 68 mm.

The imputed values may not represent the actual rainfall received during those months. Therefore, the results should be interpreted with this data-quality limitation in mind.