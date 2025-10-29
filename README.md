# 🌳 Analiza drzew w Szczecinie — EDA Project

### 🎯 Cel projektu

Celem analizy jest zbadanie danych o drzewach w mieście **Szczecin** (Polska).  
Dane pochodzą z publicznego API miasta: [dane.szczecin.eu/drzewa](https://dane.szczecin.eu/drzewa).

Projekt przedstawia:

- strukturę i czyszczenie danych
- analizę gatunków drzew
- zależność wysokości i średnicy korony
- rozmieszczenie drzew w przestrzeni miejskiej

---

### 🧰 Użyte technologie

- Python (Pandas, NumPy, Seaborn, Matplotlib)
- Folium (mapy)
- Jupyter Notebook
- JSON API (requests)

---

### 🧹 1. Przygotowanie danych

- pobranie danych z API `https://dane.szczecin.eu/drzewa/drzewa.json`
- czyszczenie kolumn (średnice, wysokości)
- obliczenie nowych zmiennych:
  - `Liczba pni`
  - `Sumaryczna średnica pnia`

---

### 📊 2. Wyniki analizy

#### 🔹 Najczęstsze gatunki

Najwięcej występujących gatunków to:

- **Klon zwyczajny**
- **Lipa drobnolistna**
- **Dąb szypułkowy**
- **Grab pospolity**

#### 🔹 Wysokość drzew

Większość drzew ma wysokość < 15 m,  
jednak pojedyncze okazy przekraczają 30 m.

#### 🔹 Kategorie danych

Drzewa parkowe są średnio o ~25% wyższe od ulicznych.

#### 🔹 Zależność wysokości od średnicy korony

Występuje lekka korelacja dodatnia —  
większe korony występują u wyższych drzew.

---

### 🗺️ 3. Mapa

W folderze `outputs/` znajduje się interaktywna mapa:

Zielone punkty oznaczają lokalizacje drzew w Szczecinie.  
Widać gęstość nasadzeń w centrum i wzdłuż głównych alei.

---

### 🧩 4. Potencjalne rozszerzenia

- Analiza zmian w czasie (kolumna `dataModyfikacji`)
- Model predykcyjny (np. przewidywanie wysokości drzewa)
- Dashboard w Tableau lub Looker Studio
- Klasteryzacja gatunków wg cech morfologicznych

---

### 📅 Źródło danych

- [https://dane.szczecin.eu/drzewa](https://dane.szczecin.eu/drzewa)
- Licencja: publiczna (Urząd Miasta Szczecin)

---

### 👤 Autor

Projekt przygotowany w ramach analizy danych publicznych (2025)  
Autor: Denys Horkavyi
