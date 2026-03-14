# Correlation and Regression Analysis using SPSS 20.0

**Supplementary Data Repository**

This repository contains all data files, figures, and output files accompanying the book chapter on **Correlation and Regression Analysis** with step-by-step demonstrations in **IBM SPSS Statistics 20.0**, using examples from agriculture, veterinary, and allied biological sciences.

---

## 👤 Author

**Dr. Kuldeep Kumar Tyagi**  
Subject Matter Expert — Animal Genetics and Breeding  
GitHub: [kuldeeptyagivet](https://github.com/kuldeeptyagivet)

---

## 📂 Repository Structure

```
correlation-regression-spss/
│
└── Chapter_01_Correlation_Regression/
    ├── data/
    │   ├── 001_Bivariate_Poultry_Data.sav
    │   ├── 001_Bivariate_Poultry_Data.xlsx
    │   ├── 001_Bivariate_Poultry_Data.csv
    │   ├── 002_Partial_Correlation_Data.sav
    │   ├── 002_Partial_Correlation_Data.xlsx
    │   └── 002_Partial_Correlation_Data.csv
    ├── output/
    │   ├── 001_Pearson_Correlation_Output.spv
    │   ├── 001_Pearson_Correlation_Output.xlsx
    │   ├── 002_Spearman_Correlation_Output.spv
    │   ├── 002_Spearman_Correlation_Output.xlsx
    │   ├── 003_Partial_Correlation_Output.spv
    │   └── 003_Partial_Correlation_Output.xlsx
    ├── figures/
    │   ├── Fig_01_Navigation_Path.png
    │   ├── Fig_02_Dialog_Box_Empty.png
    │   ├── Fig_03_Dialog_Box_Pearson.png
    │   ├── Fig_04_Dialog_Box_Spearman.png
    │   ├── Fig_05_Partial_Navigation.png
    │   ├── Fig_06_Partial_Dialog_Configured.png
    │   └── Fig_07_Partial_Options.png
    └── Assets/
        ├── QR_Corr_Reg_SPSS.svg
        └── QR_Corr_Reg_SPSS.png
```

---

## 📊 Dataset Details

### 001 — Bivariate Poultry Dataset

| Property | Details |
|---|---|
| **Species** | White Leghorn Layer Hens |
| **Sample size** | 50 birds |
| **Analysis** | Bivariate Correlation (Pearson, Spearman, Kendall) |

| Variable | Label | Unit | Scale | Decimals |
|---|---|---|---|---|
| BirdID | Bird Identifier | — | Nominal | — |
| AgeWeeks | Age of Hen | Weeks | Scale | 0 |
| BodyWeight_g | Body Weight | g | Scale | 1 |
| FeedIntake_g | Daily Feed Intake | g/day | Scale | 1 |
| EggWeight_g | Egg Weight | g | Scale | 1 |
| EggProdn_n | Weekly Egg Production | n/week | Scale | 0 |
| YolkDia_mm | Yolk Diameter | mm | Scale | 1 |
| AlbHeight_mm | Albumen Height (HU proxy) | mm | Scale | 1 |
| BCS | Body Condition Score | 1–5 | Ordinal | 0 |
| FCR | Feed Conversion Ratio | ratio | Scale | 2 |

---

### 002 — Partial Correlation Dataset

| Property | Details |
|---|---|
| **Species** | White Leghorn Layer Hens |
| **Sample size** | 60 birds |
| **Analysis** | Partial Correlation (controlling for Age) |
| **Teaching purpose** | Demonstrates spurious correlation — EggProdn × AlbHeight appear strongly correlated (r = 0.929) but partial r after controlling for Age drops to −0.070 (non-significant) |

| Variable | Label | Unit | Scale | Decimals | Role |
|---|---|---|---|---|---|
| BirdID | Bird Identifier | — | Nominal | — | ID only |
| AgeWeeks | Age of Hen | Weeks | Scale | 0 | **Control variable** |
| EggProdn_n | Weekly Egg Production | n/week | Scale | 1 | Variable 1 |
| AlbHeight_mm | Albumen Height (HU proxy) | mm | Scale | 1 | Variable 2 |
| BodyWeight_g | Body Weight | g | Scale | 1 | Variable 3 |
| FeedIntake_g | Daily Feed Intake | g/day | Scale | 1 | Variable 4 |

---

## 📥 How to Download

### Single file
Click on any file → click the **Download raw file** button (⬇ icon, top right).

### All files at once
Click the green **Code** button → **Download ZIP** → extract on your computer.

---

## 🖥️ How to Open in SPSS 20.0

**Direct open (recommended):**
```
File → Open → Data → select .sav file → Open
```
The `.sav` file opens directly with all variable names, labels, and decimal places already configured. After opening, go to **Variable View** and set measurement levels (Nominal / Ordinal / Scale) as shown in the Variable Key sheet of the corresponding `.xlsx` file.

**From Excel:**
```
File → Open → Data → Files of type: Excel → select .xlsx →
Check "Read variable names from first row" → Worksheet: Data → OK
```

---

## 📋 License

All data files and resources in this repository are released under the  
**Creative Commons Zero v1.0 Universal (CC0)** license —  
free to use, share, and adapt for any purpose without restriction.

> **Note:** All datasets are simulated (dummy) data generated for teaching and demonstration purposes only. They are not derived from any real experimental study.

---

## 📬 Contact

For questions or suggestions, please open an **Issue** in this repository.
