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
    │   ├── 001_Bivariate_Poultry_Data.sav / .xlsx / .csv
    │   ├── 002_Partial_Correlation_Data.sav / .xlsx / .csv
    │   └── 003_Simple_Regression_Data.sav / .xlsx / .csv
    ├── output/
    │   ├── 001_Pearson_Correlation_Output.spv / .xlsx
    │   ├── 002_Spearman_Correlation_Output.spv / .xlsx
    │   ├── 003_Partial_Correlation_Output.spv / .xlsx
    │   ├── 004_Simple_Regression_Output.spv / .xlsx
    │   └── 005_Multiple_Regression_Output.spv / .xlsx
    ├── figures/
    │   ├── Fig_01_Navigation_Path.png
    │   ├── Fig_02_Dialog_Box_Empty.png
    │   ├── Fig_03_Dialog_Box_Pearson.png
    │   ├── Fig_04_Dialog_Box_Spearman.png
    │   ├── Fig_05_Partial_Navigation.png
    │   ├── Fig_06_Partial_Dialog_Configured.png
    │   ├── Fig_07_Partial_Options.png
    │   ├── Fig_08_Scatter_Plot_Dialog.png
    │   ├── Fig_09_Regression_Navigation.png
    │   ├── Fig_10_Regression_Dialog.png
    │   ├── Fig_11_Regression_Statistics.png
    │   ├── Fig_12_Regression_Plots.png
    │   ├── Fig_13_Multiple_Regression_Navigation.png
    │   ├── Fig_14_Multiple_Regression_Dialog.png
    │   └── Fig_15_Multiple_Regression_Statistics.png
    └── Assets/
        ├── QR_Corr_Reg_SPSS.svg
        └── QR_Corr_Reg_SPSS.png
```

---

## 📊 Dataset Details

### 001 — Bivariate Correlation Dataset (n = 50)
**Analysis:** Bivariate Correlation — Pearson, Spearman, Kendall

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

### 002 — Partial Correlation Dataset (n = 60)
**Analysis:** Partial Correlation — controlling for Age of Hen  
**Teaching purpose:** EggProdn × AlbHeight appear strongly correlated (r = 0.929) but partial r controlling for Age drops to −0.070 (non-significant) — demonstrating spurious correlation

| Variable | Label | Unit | Scale | Role |
|---|---|---|---|---|
| BirdID | Bird Identifier | — | Nominal | ID only |
| AgeWeeks | Age of Hen | Weeks | Scale | **Control variable** |
| EggProdn_n | Weekly Egg Production | n/week | Scale | Variable 1 |
| AlbHeight_mm | Albumen Height (HU proxy) | mm | Scale | Variable 2 |
| BodyWeight_g | Body Weight | g | Scale | Variable 3 |
| FeedIntake_g | Daily Feed Intake | g/day | Scale | Variable 4 |

---

### 003 — Simple and Multiple Regression Dataset (n = 60)
**Analysis:** Simple Linear Regression + Multiple Linear Regression  
**Simple model:** EggWeight = a + b × BodyWeight (R² = 0.788)  
**Multiple model:** EggWeight = a + b₁ × BodyWeight + b₂ × Age (R² = 0.793)

| Variable | Label | Unit | Scale | Role |
|---|---|---|---|---|
| BirdID | Bird Identifier | — | Nominal | ID only |
| AgeWeeks | Age of Hen | Weeks | Scale | Independent X₂ (multiple regression) |
| BodyWeight_g | Body Weight | g | Scale | **Independent X / X₁** |
| EggWeight_g | Egg Weight | g | Scale | **Dependent Y** |

---

## 📥 How to Download

**Single file:** Click filename → **Download raw file** button (⬇ icon, top right)

**All files:** Click green **<> Code** button → **Download ZIP** → extract on your computer

---

## 🖥️ How to Open in SPSS 20.0

```
File → Open → Data → select .sav file → Open
```
After opening, go to **Variable View** and set measurement levels (Nominal / Ordinal / Scale) as shown in the Variable Key sheet of the corresponding `.xlsx` file.

---

## 📋 License

Released under **Creative Commons Zero v1.0 Universal (CC0)** — free to use, share, and adapt.

> **Note:** All datasets are simulated (dummy) data generated for teaching and demonstration purposes only.

---

## 📬 Contact

For questions or suggestions, please open an **Issue** in this repository.
