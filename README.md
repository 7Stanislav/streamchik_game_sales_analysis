# Исследование интернет-магазина компьютерных игр "Стримчик"

## Описание проекта

Данный проект выполнен для интернет-магазина «Стримчик», который продаёт компьютерные игры по всему миру. Основная цель — выявить определяющие успешность игры закономерности на основе исторических данных о продажах, оценках пользователей и экспертов, жанрах и платформах. Результаты анализа позволят спланировать рекламные кампании и сделать ставку на потенциально популярные продукты в 2017 году, используя данные до конца 2016 года.

В наборе данных также присутствует аббревиатура ESRB (Entertainment Software Rating Board) — ассоциация, определяющая возрастной рейтинг компьютерных игр.

## Используемые данные

В проекте используется файл `games.csv`, содержащий следующую информацию:
* `Name` — название игры
* `Platform` — платформа (например, Xbox, PlayStation)
* `Year_of_Release` — год выпуска игры
* `Genre` — жанр игры
* `NA_sales` — продажи в Северной Америке (млн USD)
* `EU_sales` — продажи в Европе (млн USD)
* `JP_sales` — продажи в Японии (млн USD)
* `Other_sales` — продажи в других странах (млн USD)
* `Critic_Score` — оценка критиков (максимум 100)
* `User_Score` — оценка пользователей (максимум 10)
* `Rating` — возрастной рейтинг от ESRB

## Ход исследования

Проект включает следующие основные этапы:

1.  **Первичный анализ и подготовка данных:**
    * Загрузка и обзор данных (типы, пропуски, дубликаты).
    * Приведение названий столбцов к нижнему регистру.
    * Преобразование типов данных (например, года выпуска, оценок).
    * Обработка пропусков в различных столбцах (заполнение или удаление).
    * Расчет общей суммы продаж для каждой игры по всем регионам (`total_sales`).

2.  **Исследовательский анализ данных (EDA):**
    * Анализ динамики выпуска игр и общих продаж по годам.
    * Изучение "жизненного цикла" платформ и определение актуального периода данных (с 2014 года) для дальнейшего анализа.
    * Исследование распределения продаж игр по платформам с использованием боксплотов.
    * Анализ влияния оценок критиков и пользователей на продажи игр.
    * Изучение распределения продаж по жанрам.

3.  **Региональный анализ:**
    * Определение топ-5 наиболее популярных платформ в каждом регионе (Северная Америка, Европа, Япония).
    * Выявление топ-5 наиболее популярных жанров в каждом регионе.
    * Анализ влияния возрастного рейтинга ESRB на продажи в каждом регионе.

4.  **Проверка статистических гипотез:**
    * Сравнение средних пользовательских рейтингов для платформ Xbox One и PC.
    * Сравнение средних пользовательских рейтингов для жанров Action и Sports.

5.  **Общий вывод и рекомендации:**
    * Формулировка ключевых выводов на основе проведенного анализа.
    * Разработка практических рекомендаций для интернет-магазина «Стримчик» по планированию рекламных кампаний и определению перспективных продуктов на 2017 год.

## Ключевые выводы и рекомендации

На основе проведенного анализа данных интернет-магазина "Стримчик" были выявлены следующие закономерности и сформулированы рекомендации:

* **Жизненный цикл платформ:** Продажи игр на разных платформах имеют четкие жизненные циклы. Для прогнозирования на 2017 год критически важно фокусироваться на данных последних актуальных лет (с 2014 года), так как более старые данные не отражают текущих трендов.
* **Влияние оценок:** Оценки критиков и пользователей могут по-разному коррелировать с продажами. В ходе анализа было установлено, что [здесь можно будет конкретизировать, например: "оценки критиков, как правило, имеют более сильную положительную корреляцию с продажами, чем оценки пользователей"]. Это указывает на важность профессионального признания для коммерческого успеха игры.
* **Прибыльные жанры:** Определенные жанры демонстрируют стабильно высокие медианные продажи, что делает их более предсказуемыми и потенциально прибыльными. Однако, для выявления "хитов" необходимо также учитывать выбросы в продажах, так как именно они указывают на исключительно успешные игры.
* **Региональные особенности:**
    * **Платформы:** Топ-платформы значительно различаются по регионам. Например, [здесь можно будет конкретизировать, например: "PlayStation и Xbox доминируют в Северной Америке и Европе, в то время как в Японии популярность сохраняют свои, уникальные платформы"].
    * **Жанры:** Предпочтения по жанрам также сильно зависят от региона. [Здесь можно будет конкретизировать, например: "В Северной Америке и Европе популярны Action и Shooter, тогда как в Японии преобладают Role-Playing и Puzzle."].
    * **Возрастные рейтинги ESRB:** Влияние ESRB-рейтингов на продажи варьируется в зависимости от региона, что указывает на различия в целевой аудитории и культурных особенностях.
* **Статистические различия:** Гипотезы о сравнении средних пользовательских рейтингов для различных платформ (например, Xbox One и PC) и жанров (например, Action и Sports) показали [здесь можно будет конкретизировать, например: "статистически значимые различия" или "отсутствие значимых различий"], что помогает глубже понять предпочтения аудитории.

**Рекомендации для интернет-магазина "Стримчик" на 2017 год:**

* **Приоритет актуальным платформам:** Сфокусировать рекламные бюджеты на актуальных и растущих платформах, игнорируя те, чей жизненный цикл подходит к концу.
* **Учет оценок:** При планировании закупок и продвижения игр учитывать как оценки критиков, так и пользовательские, отдавая приоритет тем, что демонстрируют более сильную корреляцию с продажами.
* **Целевое продвижение по жанрам:** Разрабатывать рекламные кампании с учетом самых прибыльных жанров, а также анализировать уникальные особенности хитов для выявления их успеха.
* **Региональная адаптация:** Маркетинговые и продуктовые стратегии должны быть строго адаптированы под региональные предпочтения в платформах, жанрах и возрастных рейтингах. Универсальный подход может быть неэффективен.

## Используемые технологии

* Python
* Pandas
* Matplotlib
* Seaborn
* SciPy
* Jupyter Notebook

## Как запустить проект

Для воспроизведения анализа:
1.  **Клонируйте репозиторий:** `git clone https://github.com/7Stanislav/streamchik_game_sales_analysis`
2.  **Установите необходимые библиотеки:** Убедитесь, что у вас установлены `pandas`, `matplotlib`, `seaborn`, `scipy`. Если нет, установите их:
    `pip install pandas matplotlib seaborn scipy`
3.  **Загрузите данные:** Файл `games.csv` должен находиться в той же директории, что и Jupyter Notebook.
4.  **Запустите Jupyter Notebook/Lab:** Откройте `project.ipynb` в Jupyter Notebook или JupyterLab.
5.  **Выполните все ячейки:** Запустите все ячейки блокнота по порядку.
