# *Отчет*
Работу выполнили студенты 4ИВТ(1):
- Сорокина Ирина
- Чалапко Егор
- Шафорост Наталья 
---
# *Содержание*
- Что такое DevOps простыми словами
- Как происходит разработка по подходу DevOps
  - Формулирование требований и проектирование
  - Разработка
  - Запуск конвейера CI/CD
  - Неприрывное тестирование
  - Неприрывное развертывание
  - Неприрывный мониторинг
---
## Что такое DevOps простыми словами ###
Классический процесс разработки состоит из трех разделенных этапов:
  - сначала команда программистов — Dev — пишет код и делает его сборку;
  - потом команда тестировщиков — QA/QC — берет код от программистов и тестирует его;
  - наконец, команда администраторов — Ops — устанавливает протестированный код на «боевые» серверы, то есть преподносит его пользователям.

DevOps — это особый подход к организации команд разработки. Его суть в том, что разработчики, тестировщики и администраторы работают в едином потоке — не отвечают каждые за свой этап, а вместе работают над выходом продукта и стараются автоматизировать задачи своих отделов, чтобы код переходил между этапами без задержек. В DevOps ответственность за результат распределяется между всей командой.
![картинка](https://i0.wp.com/mcsjournal.ru/wp-content/uploads/2021/02/Razrabotka.png?w=1200&ssl=1)
Чтобы DevOps работал, нужно наладить непрерывную связь — конвейер между разработчиками, тестировщиками и администраторами. Для этого нужны инструменты автоматизации, которые помогут эффективнее передавать код, тестировать его и развертывать на серверах.
## Как происходит разработка по подходу DevOps
### 1. Формулирование требований и проектирование
Планируется разработать приложение использующее технологии машинного обучения. Оно будет классифицировать цветки ириса из выборки Фишера, относя их к одному из четырёх видов: ирис щетинистый (iris setosa), ирис версиколор (iris versicolor), ирис виргинский (iris virginica).
- Понадобятся библиотеки streamlit, pandas и scikit-learn.
- Приложение будет состоять из двух больших частей: Front-end и Back-end
- Во фронтенд-части приложения, а именно, на веб-странице, будет боковая панель, находящаяся слева, в которой можно будет вводить входные параметры модели, которые связаны с характеристиками цветков ириса: длина лепестка (petal length), ширина лепестка (petal width), длина чашелистика (sepal length), ширина чашелистика (sepal width). Эти данные будут передаваться бэкенду, где предварительно обученная модель будет классифицировать цветки, используя заданные характеристики. Фактически, речь идёт о функции, которая, получая характеристики цветка, возвращает его вид. Результаты классификации отправляются фронтенду.

- В бэкенд-части приложения то, что ввёл пользователь, сохраняется в датафрейме, который будет использоваться в виде тестовых данных для модели. Потом будет построена модель для обработки данных. В ней будет применяться алгоритм «случайный лес» из библиотеки scikit-learn. И наконец, модель будет применена для классификации данных, введённых пользователем, то есть — для определения вида цветка. Кроме того, вместе со сведениями о виде цветка, будут возвращаться и данные о прогностической вероятности. Это позволит нам определить степень достоверности результатов классификации.

### 2. Разработка
### 3. Запуск конвейера CI/CD
### 4. Непрерывное тестирование
### 5. Неприрывное развертывание
### 6. Неприрывный мониторинг
