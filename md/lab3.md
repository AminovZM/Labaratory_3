---
# Front matter
lang: ru-RU
title: "ОТЧЕТ ПО ЛАБОРАТОРНОЙ РАБОТЕ №3"
subtitle: "Введение в работу с Octave"
author: "Аминов Зулфикор Мирзокаримович"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Ход работы:

# 3.4.1. Простейшие операции

1. Включите журналирование сесии

![рисунка 1](img/3.4.1/1.PNG){ #fig:001 width=70% }

2. Поскольку оператор diary является переключателем, то достаточно ввести

![рисунка 2](img/3.4.1/2.PNG){ #fig:001 width=70% }

3. Octave можно использовать как простейший калькулятор. Вычислим выражение

![рисунка 3](img/3.4.1/3.PNG){ #fig:001 width=70% }

4. Зададим вектор-строку (ковектор):

![рисунка 4](img/3.4.1/4.PNG){ #fig:001 width=70% }

5. Аналогично можно задать вектор-столбец (вектор):

![рисунка 5](img/3.4.1/5.PNG){ #fig:001 width=70% }

6. Теперь зададим матрицу:

![рисунка 6](img/3.4.1/6.PNG){ #fig:001 width=70% }

# 3.4.2. Операции с векторами

1. Зададим два вектора-столбца:

![рисунка 7](img/3.4.2/1.PNG){ #fig:001 width=70% }

2. Сложение векторов:

![рисунка 8](img/3.4.2/2.PNG){ #fig:001 width=70% }

3. Скалярное умножение векторов:

![рисунка 9](img/3.4.2/3.PNG){ #fig:001 width=70% }

4. Векторное умножение векторов:

![рисунка 10](img/3.4.2/4.PNG){ #fig:001 width=70% }

5. Норма вектора:

![рисунка 11](img/3.4.2/5.PNG){ #fig:001 width=70% }

# 3.4.3. Вычисление проектора

1. Введём два вектора-строки:

![рисунка 12](img/3.4.3/1.PNG){ #fig:001 width=70% }

2. Вычислим проекцию вектора 𝑢⃗ на вектор 𝑣.⃗

![рисунка 13](img/3.4.3/2.PNG){ #fig:001 width=70% }

# 3.4.4. Матричные операции

1. Введём матрицы ̂ A и ̂B:

![рисунка 14](img/3.4.4/1.PNG){ #fig:001 width=70% }

2. Вычислим произведение матриц ̂ A ̂B:

![рисунка 15](img/3.4.4/2.PNG){ #fig:001 width=70% }

3. Вычислим произведение матриц1 ̂BTÂ :

![рисунка 16](img/3.4.4/3.PNG){ #fig:001 width=70% }

4. Вычислим 2Â − 4I

![рисунка 17](img/3.4.4/4.PNG){ #fig:001 width=70% }

5. Найдём определитель |Â|:

![рисунка 18](img/3.4.4/5.PNG){ #fig:001 width=70% }

6. Найдём обратную матрицу Â−1:

![рисунка 19](img/3.4.4/6.PNG){ #fig:001 width=70% }

7. Найдём собственные значения1 матрицы Â :

![рисунка 20](img/3.4.4/7.PNG){ #fig:001 width=70% }

8. Найдём ранг матрицы Â :

![рисунка 21](img/3.4.4/8.PNG){ #fig:001 width=70% }

# 3.4.5. Построение простейших графиков

Построим график функции sin 𝑥 на интервале [0, 2π].

1. Создадим вектор значений 𝑥:

![рисунка 22](img/3.4.5/1.PNG){ #fig:001 width=70% }

2. Зададим вектор 𝑦 = sin 𝑥:

![рисунка 23](img/3.4.5/2.PNG){ #fig:001 width=70% }

3. Построим график:

![рисунка 24](img/3.4.5/3.PNG){ #fig:001 width=70% }
![рисунка 25](img/3.4.5/3.1.PNG){ #fig:001 width=70% }

4. Улучшим внешний вид графика. Сначала очистим получившийся график:

![рисунка 26](img/3.4.5/4.PNG){ #fig:001 width=70% }
![рисунка 27](img/3.4.5/4.1.PNG){ #fig:001 width=70% }

5. Зададим красный цвет для линии и сделаем её потолще:

![рисунка 28](img/3.4.5/5.PNG){ #fig:001 width=70% }
![рисунка 29](img/3.4.5/5.1.PNG){ #fig:001 width=70% }

6. Подгоним диапазон осей:

![рисунка 30](img/3.4.5/6.PNG){ #fig:001 width=70% }

7. Нарисуем сетку:

![рисунка 31](img/3.4.5/6.1.PNG){ #fig:001 width=70% }
![рисунка 32](img/3.4.5/7.PNG){ #fig:001 width=70% }
![рисунка 33](img/3.4.5/7.1.PNG){ #fig:001 width=70% }

8. Подпишем оси:

![рисунка 34](img/3.4.5/8.PNG){ #fig:001 width=70% }
![рисунка 35](img/3.4.5/8.1.PNG){ #fig:001 width=70% }

9. Сделаем заголовок графика:

![рисунка 36](img/3.4.5/9.PNG){ #fig:001 width=70% }
![рисунка 37](img/3.4.5/9.1.PNG){ #fig:001 width=70% }

10. Зададим легенду:

![рисунка 38](img/3.4.5/10.PNG){ #fig:001 width=70% }
![рисунка 39](img/3.4.5/10.1.PNG){ #fig:001 width=70% }

# 3.4.6. Два графика на одном чертеже

Начертим два графика на одном чертеже.

1. Очистим память и рабочую область фигуры:

![рисунка 40](img/3.4.6/1.PNG){ #fig:001 width=70% }
![рисунка 41](img/3.4.6/1.1.PNG){ #fig:001 width=70% }

2. Зададим два вектора:

![рисунка 42](img/3.4.6/2.PNG){ #fig:001 width=70% }

3. Начертим эти точки, используя кружочки как маркеры:

![рисунка 43](img/3.4.6/3.PNG){ #fig:001 width=70% }
![рисунка 44](img/3.4.6/3.1.PNG){ #fig:001 width=70% }

4. Чтобы добавить к нашему текущему графику ещё один, нужно использовать команду:

![рисунка 45](img/3.4.6/4.PNG){ #fig:001 width=70% }

5. Добавим график регрессии:

![рисунка 46](img/3.4.6/5.PNG){ #fig:001 width=70% }
![рисунка 47](img/3.4.6/5.1.PNG){ #fig:001 width=70% }

6. Зададим сетку, оси и легенду:

![рисунка 48](img/3.4.6/6.PNG){ #fig:001 width=70% }
![рисунка 49](img/3.4.6/6.1.PNG){ #fig:001 width=70% }

# 3.4.7. График *y = x^2sinx*

Построим график y = x^2sinx

1. Очистим память и рабочую область фигуры:

![рисунка 50](img/3.4.7/1.PNG){ #fig:001 width=70% }
![рисунка 51](img/3.4.7/1.1.PNG){ #fig:001 width=70% }

2. Зададим вектор 𝑥:

![рисунка 52](img/3.4.7/2.PNG){ #fig:001 width=70% }

3. Построим график 𝑦 = 𝑥2 sin 𝑥:

![рисунка 53](img/3.4.7/3.PNG){ #fig:001 width=70% }

4. Построим график 𝑦 = 𝑥2 sin 𝑥, используя поэлементное возведение в степень .^ и поэлементное умножение .*:

![рисунка 54](img/3.4.7/4.PNG){ #fig:001 width=70% }
![рисунка 55](img/3.4.7/4.1.PNG){ #fig:001 width=70% }

5. Сохраним графики в виде файлов (отметьте два разных формата вызова функции):

Сохранил.

# 3.4.8. Сравнение циклов и операций с векторами

Сравним эффективность работы с циклами и операций с векторами. Для этого вычислим сумму:

1. Очистим память и рабочую область фигуры:

![рисунка 56](img/3.4.8/1.PNG){ #fig:001 width=70% }

2. Вычислим сумму (3.1) с помощью цикла. Создадим файл loop_for.m:

![рисунка 57](img/3.4.8/2.PNG){ #fig:001 width=70% }

3. Вычислим сумму (3.1) с помощью операций с векторами. Создадим файл loop_vec.m:

![рисунка 58](img/3.4.8/3.PNG){ #fig:001 width=70% }

4. Завершим запись в файл:

![рисунка 59](img/3.4.8/4.PNG){ #fig:001 width=70% }

### 3.5. Вывод:

Я научился работать с простейшей операциям в octave.
