# 🇵🇰 Pakistan Crop Yield Prediction Project

## 🎯 Objective  
Predict district-level crop yields in Pakistan using:
- Soil health data from **Punjab Soil Fertility Labs**
- Weather patterns from **PMD (Pakistan Meteorological Department)**
- Satellite NDVI from **SUPARCO**

**Example Output:**  
*"Wheat yield prediction for Punjab (2023-24) with fertilizer recommendations"*

---

## 🌾 Dataset Sources (Pakistan-Specific)

| **Source** | **Data Type** | **Access Method** |
|------------|---------------|-------------------|
| [Punjab Soil Health Portal](http://soilhealth.punjab.gov.pk) | pH, N-P-K levels | Web scraping/PDF parsing |
| [PMD Climate Portal](https://www.pmd.gov.pk/climate) | Rainfall/Temperature | CSV download |
| SUPARCO | 10m resolution NDVI | Google Earth Engine |
| [Pakistan Bureau of Statistics](http://www.pbs.gov.pk/agri-statistics) | Historical yields | PDF reports |

**Sample Data Format:**
```csv
district,soil_ph,n_level,p_level,k_level,rainfall(mm),yield(kg/acre)
"Faisalabad",7.2,45,12,180,350,3200
"Multan",8.1,32,8,210,290,1700
