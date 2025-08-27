# Cosmetic Ingredients Dataset (Lite) by BEAUTEE

Open dataset of cosmetic ingredients curated by [BEAUTEE](https://beautee.ru) — service for analyzing cosmetic product compositions.

This **lite version** includes public identifiers for ingredients (INCI, COSING ID, CAS, EINECS, PubChem ID, synonyms).  
It is intended for researchers, data scientists and developers who want to work with standardized cosmetic ingredient identifiers.

👉 Full ingredient analysis with safety tags, skin type recommendations, and product breakdowns is available at [beautee.ru](https://beautee.ru).

---

## 📂 Dataset structure

`ingredients.csv` / `ingredients.json`

Columns:
- **INCI** — International Nomenclature of Cosmetic Ingredients  
- **COSING_ID** — ID from the official EU CosIng database  
- **CAS** — CAS Registry Number  
- **EINECS** — European Community number  
- **PubChem_ID** — PubChem compound identifier  

---

## 📝 Example rows

| NAME INCI   | COSING_ID | CAS      | EINECS   | PubChem_ID |
|-------------|-----------|----------|----------|------------|
| Glycerin    | 12345     | 56-81-5  | 200-289-5| 753        |
| Niacinamide | 54321     | 98-92-0  | 202-713-4| 936        |

---

## ⚡ Quick start (Python)

```python
import pandas as pd

# Load dataset
df = pd.read_csv("ingredients.csv")

# Show first rows
print(df.head())

# Example: filter by CAS
cas = "56-81-5"
print(df[df["CAS"] == cas])
```

## 🔗 Related resources
[CosIng database (EU)](https://ec.europa.eu/growth/tools-databases/cosing/)
[PubChem](https://pubchem.ncbi.nlm.nih.gov/)
[ECHA (EINECS)](https://echa.europa.eu/information-on-chemicals/ec-inventory)
[BEAUTEE: cosmetic product analysis](https://beautee.ru/)

## 📜 License
Released under the MIT License
Copyright (c) 2025 BEAUTEE.

You are free to use, copy, modify, merge, publish and distribute this dataset.
Please retain the copyright notice and link to [beautee.ru](https://beautee.ru/)

## 🙌 About BEAUTEE

[BEAUTEE](https://beautee.ru/) is an service for analyzing cosmetic product compositions.
- 🔍 Free basic ingredient analysis
- 🤖 Personalized breakdowns with skin/hair type recommendations
- 📚 Ingredient catalog and product database

---

## 🇷🇺 Описание на русском

**BEAUTEE** — это сервис анализа косметики.  
Мы делаем разборы составов косметических средств, чтобы помочь вам выбрать лучшее:  
- Бесплатный базовый разбор состава  
- Персонализированные рекомендации по типу кожи и волос  
- Каталог ингредиентов и продуктов  

Этот репозиторий содержит **упрощённую (lite) версию базы ингредиентов**: INCI, CAS, EINECS, PubChem ID и CosIng ID.  
Полные данные с описанием функций ингредиентов, рисками и рекомендациями доступны на сайте [beautee.ru](https://beautee.ru).
