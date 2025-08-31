# 📊 Streamchik Game Sales Analysis / Исследование интернет-магазина компьютерных игр «Стримчик»

## Description / Описание
**EN:**  
This project was conducted for the online game store *Streamchik*, which sells video games worldwide. The primary goal was to identify the key factors driving game success using historical data on sales, user and critic reviews, genres, and platforms. The insights gained help plan marketing campaigns and focus on potentially popular products in 2017, based on data up to the end of 2016.

The dataset also includes ESRB (Entertainment Software Rating Board) ratings, which provide information about the target audience age categories.  

**RU:**  
Данный проект выполнен для интернет-магазина «Стримчик», который продаёт компьютерные игры по всему миру. Основная цель — выявить определяющие успешность игры закономерности на основе исторических данных о продажах, оценках пользователей и экспертов, жанрах и платформах. Результаты анализа позволят спланировать рекламные кампании и сделать ставку на потенциально популярные продукты в 2017 году, используя данные до конца 2016 года.  

В наборе данных также присутствует аббревиатура ESRB (Entertainment Software Rating Board) — ассоциация, определяющая возрастной рейтинг компьютерных игр.  

---

## Dataset / Используемые данные
**EN:**  
The dataset (`games.csv`) contains:  
- `Name` — game title  
- `Platform` — platform (Xbox, PlayStation, etc.)  
- `Year_of_Release` — release year  
- `Genre` — genre  
- `NA_sales`, `EU_sales`, `JP_sales`, `Other_sales` — regional sales (in million USD)  
- `Critic_Score` — critic score (0–100)  
- `User_Score` — user score (0–10)  
- `Rating` — ESRB rating  

**RU:**  
В проекте используется файл `games.csv`, содержащий следующую информацию:  
- `Name` — название игры  
- `Platform` — платформа (например, Xbox, PlayStation)  
- `Year_of_Release` — год выпуска игры  
- `Genre` — жанр игры  
- `NA_sales`, `EU_sales`, `JP_sales`, `Other_sales` — продажи в соответствующих регионах (в млн USD)  
- `Critic_Score` — оценка критиков (максимум 100)  
- `User_Score` — оценка пользователей (максимум 10)  
- `Rating` — возрастной рейтинг от ESRB  

---

## Research Workflow / Ход исследования
**EN:**  
1. **Data Preparation**  
   - Loading and reviewing data (types, missing values, duplicates)  
   - Standardizing column names  
   - Converting data types (e.g., release year, scores)  
   - Handling missing values (imputation/removal)  
   - Calculating total sales per game  

2. **Exploratory Data Analysis (EDA)**  
   - Analyzing game release dynamics and sales trends  
   - Identifying platform life cycles (focusing on 2014+)  
   - Boxplot analysis of sales distribution by platform  
   - Studying correlations between scores (critics/users) and sales  
   - Genre sales distribution analysis  

3. **Regional Analysis**  
   - Top-5 platforms by region (NA, EU, JP)  
   - Top-5 genres by region  
   - ESRB ratings impact on sales  

4. **Hypothesis Testing**  
   - Compare user ratings between Xbox One and PC  
   - Compare user ratings between Action and Sports genres  

5. **Conclusions & Recommendations**  

**RU:**  
1. **Первичный анализ и подготовка данных**  
   - Загрузка и обзор данных  
   - Приведение названий столбцов к нижнему регистру  
   - Преобразование типов данных  
   - Обработка пропусков  
   - Расчет общей суммы продаж  

2. **EDA (исследовательский анализ)**  
   - Анализ динамики выпуска игр  
   - Определение «жизненного цикла» платформ (с 2014 года)  
   - Анализ продаж по платформам и жанрам  
   - Влияние оценок критиков/пользователей  

3. **Региональный анализ**  
   - Топ-5 платформ и жанров в регионах  
   - Влияние ESRB на продажи  

4. **Проверка гипотез**  
   - Сравнение рейтингов пользователей между платформами  
   - Сравнение рейтингов жанров  

5. **Итоговые выводы и рекомендации**  

---

## Key Findings & Recommendations / Ключевые выводы и рекомендации
**EN:**  
- **Platform life cycle:** focus on recent years (2014+) for accurate forecasts.  
- **Critic vs User Scores:** critic scores often correlate stronger with sales.  
- **Profitable Genres:** certain genres show consistently higher median sales.  
- **Regional Specifics:** preferences vary by region (e.g., PlayStation/Xbox in NA & EU vs Role-Playing in JP).  
- **ESRB Ratings:** impact differs across regions.  
- **Hypothesis Testing:** provided statistical insights into platform and genre preferences.  

**RU:**  
- **Жизненный цикл платформ:** учитывать данные последних лет (с 2014).  
- **Оценки критиков и пользователей:** критики сильнее влияют на продажи.  
- **Жанры:** есть прибыльные и предсказуемые жанры.  
- **Регионы:** платформы и жанры сильно различаются по регионам.  
- **Рейтинги ESRB:** эффект разный в зависимости от аудитории.  
- **Статистические гипотезы:** помогли глубже понять предпочтения пользователей.  

---

## Technologies / Используемые технологии
- Python  
- Pandas  
- Matplotlib  
- Seaborn  
- SciPy  
- Jupyter Notebook  

---

## How to Run / Как запустить проект
**EN:**  
1. Clone repository:  
   ```
   git clone https://github.com/7Stanislav/streamchik_game_sales_analysis
   ```  
2. Install dependencies:  
   ```
   pip install pandas matplotlib seaborn scipy
   ```  
3. Place `games.csv` in the project directory.  
4. Open `project.ipynb` in Jupyter Notebook/Lab.  
5. Run all cells.  

**RU:**  
1. Клонируйте репозиторий:  
   ```
   git clone https://github.com/7Stanislav/streamchik_game_sales_analysis
   ```  
2. Установите зависимости:  
   ```
   pip install pandas matplotlib seaborn scipy
   ```  
3. Поместите `games.csv` в директорию проекта.  
4. Откройте `project.ipynb` в Jupyter Notebook или JupyterLab.  
5. Запустите все ячейки по порядку.  
