# 🌍 Analiza zanieczyszczenia powietrza – dane WHO

## 📌 Opis projektu
Projekt obejmuje analizę eksploracyjną danych (EDA) oraz modelowanie predykcyjne na podstawie danych dotyczących jakości powietrza pochodzących z bazy **Światowej Organizacji Zdrowia (WHO)**.

Analiza została przeprowadzona na trzech poziomach agregacji:
- regionów (WHO),
- krajów,
- miast.

Celem projektu jest:
- zrozumienie rozkładu i zmienności zanieczyszczeń powietrza,
- identyfikacja trendów w czasie,
- porównanie poziomów zanieczyszczeń pomiędzy regionami, krajami i miastami,
- zbudowanie modelu predykcyjnego dla poziomu PM2.5.

---

## 📊 Zakres danych
Zbiór danych zawiera informacje o poziomie zanieczyszczeń powietrza w różnych lokalizacjach na świecie.

### Główne zmienne:
- **PM2.5 (μg/m3)** – drobne cząstki pyłu zawieszonego,
- **PM10 (μg/m3)** – większe cząstki pyłu,
- **NO2 (μg/m3)** – dwutlenek azotu,
- **Measurement Year** – rok pomiaru,
- **City or Locality** – miasto,
- **WHO Country Name** – kraj,
- **WHO Region** – region WHO,
- **temporal coverage (%)** – pokrycie czasowe danych.

---

## 🔍 Zakres analizy (EDA)

### 📌 Analiza jakości danych
- identyfikacja braków danych,
- analiza braków w podziale na regiony i kraje,
- ocena kompletności danych.

### 📌 Imputacja danych
- imputacja brakujących wartości **PM2.5** na podstawie relacji z PM10,
- uzupełnianie braków na poziomie regionów i lat,
- analiza wpływu imputacji na wyniki.

### 📌 Analiza rozkładów
- histogramy i boxploty dla PM2.5, PM10, NO2,
- identyfikacja wartości odstających,
- porównanie rozkładów między regionami.

### 📌 Analiza trendów czasowych
- zmiany poziomu zanieczyszczeń w czasie,
- trendy dla regionów, krajów i miast,
- analiza liczby obserwacji w czasie.

### 📌 Porównania między poziomami
- ranking regionów według zanieczyszczeń,
- ranking krajów i miast,
- analiza najbardziej zanieczyszczonych lokalizacji.

### 📌 Analiza zależności
- korelacje między PM2.5, PM10 i NO2,
- wizualizacja zależności (scatter ploty),
- macierz korelacji.

### 📌 Wizualizacje
- wykresy statyczne (Matplotlib, Seaborn),
- mapy (Plotly),
- dashboardy interaktywne (ipywidgets).

---

## 🤖 Modelowanie predykcyjne

W projekcie zbudowano model **Random Forest Regressor**, którego celem było przewidywanie poziomu **PM2.5**.

### 📌 Wykorzystane cechy:
- PM10,
- NO2,
- pokrycie czasowe danych,
- rok pomiaru,
- region (zakodowany jako zmienna kategoryczna).

### 📌 Metryki:
- R² (train i test),
- RMSE,
- MAE.

## 🛠️ Technologie

Projekt został zrealizowany z wykorzystaniem:
- Python
- Pandas
- GeoPandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Scikit-learn
- Jupyter Notebook

---

## 👤 Autor
Projekt wykonany w ramach pracy projektowej z zakresu analizy danych i uczenia maszynowego.
