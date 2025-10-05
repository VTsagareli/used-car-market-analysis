
# 🚗 Used Car Market Analysis Dashboard (Germany, AutoScout24)

An interactive Tableau dashboard analyzing a German used car listings dataset (from Kaggle) to uncover trends in pricing, mileage, vehicle age, fuel type, and transmission. The dashboard lets users filter and explore how these features vary across brands and registration years.

📊 **[View the Live Dashboard on Tableau Public »](https://public.tableau.com/shared/RSSX3S2P5?:display_count=n&:origin=viz_share_link)**  
📁 **[View the Dataset on Kaggle »](https://www.kaggle.com/datasets/wspirat/germany-used-cars-dataset-2023)**

---

## 🧠 Project Objective

The purpose of this project is to provide a clean, intuitive dashboard that helps users understand the dynamics of the German used car market. Key focus questions include:

- What is the median price, mileage, and age of used cars in this dataset?  
- How are vehicles distributed by fuel type and transmission?  
- What brands command higher prices, and how does price decline across registration years?  
- How do mileage and age interplay across listings?

---

## 🛠 Data Cleaning & Preparation (Python)

Data preparation was done in Python (using Pandas) to ensure integrity and consistency. Major steps included:

- Parsing and converting textual fields (e.g. `"9,4 l/100 km"`) into numeric formats  
- Handling missing or nonstandard values in `price`, `mileage`, `fuel_type`, and `power`  
- Standardizing categories for fuel types and transmissions  
- Engineering new fields: `car_age`, `mileage_k` (mileage in thousands), `price_per_kw`, and `ev_has_range_data`  
- Exporting the cleaned dataset for ingestion into Tableau

---

## 📈 Dashboard Structure & Visual Flow

The dashboard is organized to support an intuitive narrative:

### 🔹 Top Section – KPIs  
- Median Price  
- Median Mileage  
- Median Year of Registration  
- Percentage of Electric Vehicles  

### 🔹 Market Composition  
- Pie chart: Transmission Type (Manual, Automatic, Semi-automatic)  
- Pie chart: Fuel Type (Petrol, Diesel, Hybrid, Electric)  

### 🔹 Detailed Insights  
- Bar chart: Median Price by Brand  
- Bar chart: Median Mileage by Year (or per registration year)  

### 🔹 Interactive Controls  
Filters available across all visuals:

- Year / Registration Year
- Mileage (range slider, in thousands)    

Additional filters such as mileage, brand, fuel type, etc. can be added depending on user needs.

---

## 💡 Key Insights

- A significant proportion of listings are **Petrol or Diesel** vehicles.  
- Only a small share of EVs appears in the dataset.  
- Median values paint a clearer picture than averages in this skewed dataset:  
  - Median price is noticeably lower than the average.  
  - Mileage and age distributions are right-skewed, indicating many newer, low-mileage vehicles.  
- Some brands consistently command higher median prices.  
- Mileage tends to increase with older registration years, though with some variation.

---

## 🚀 Future Enhancements

- Add predictive modeling (price estimation based on features)  
- Integrate geographical data for regional insights  
- Display trend of EV adoption over time  
- Add benchmarks (e.g. compare with new car pricing, residual values)  
- Support export of filtered data or additional detail views

---

## 📌 Tools & Technologies

| Tool/Technology    | Purpose                              |
|--------------------|--------------------------------------|
| Python + Pandas    | Data cleaning, feature engineering   |
| Tableau            | Dashboard creation and visualization |
| Kaggle (source)    | Dataset provision                    |

---

## 👤 Author

**[Vakho Tsagareli]** – Aspiring Data Analyst
📧 tsagareli.v@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/vakhtang-tsagareli/) | 🔗 [Portfolio](https://www.datascienceportfol.io/tsagareliv)  
