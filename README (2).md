# PLP Data Analysis Assignment 2: Rainfall Advisory

**Analyst:** Jessca Waithera Gichangi  
**PLP Cohort:** [1 million devs]

## Project summary

This project analyses monthly rainfall readings for Nairobi, Nakuru, Kisumu, Mombasa and Machakos to help a farmer-support NGO communicate practical planting windows. The Machakos station's raw text values are cleaned with specific `ValueError` handling and invalid months are imputed using the rounded mean of valid readings. NumPy is then used to calculate annual rainfall totals, monthly averages, wettest months, dry-month counts and the strongest consecutive two-month planting window for each county.

## How to run

Open `rainfall_analysis.ipynb` in [Google Colab](https://colab.research.google.com/github/Gichangi-J/plp-da-a2-rainfall-advisory/blob/main/rainfall_analysis.ipynb), or run it locally with Jupyter Notebook. Install the listed dependency with `pip install -r requirements.txt`, then restart the kernel and run all cells from top to bottom. The notebook creates `rainfall_summary.csv` in the same working directory.

## Planting advisory

- Use the county-specific two-month planting windows in `rainfall_summary.csv` as planning guidance, and confirm timing with current local forecasts.
- In counties with multiple months below 50 mm, encourage water conservation, soil-moisture retention and suitable drought-tolerant crops.
- Treat the recommendations cautiously because Machakos April and September values were imputed from the mean of its valid readings, and monthly totals do not show the timing or intensity of individual rain events.
