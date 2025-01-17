## Курс "Практична журналістика та візуалізація даних""
### (із використанням мови програмування R)

УКУ, "Медіакомунікації", 2019 рік


Ідея курсу: Концептуально етапи курсу співпадають з базовими етапами будь якого проекту з візуалізації 
даних --- отримання даних-обробка-аналіз-візуалізація. Однак ми використовуємо "забігання"" - ми пробуємо щось нове/складне, дуже швидко. Потім пізніше повертаємося до цієї теми. І третє - практикуємося, помиляємося і виправляємо помилки.

Головна мета: навчити не боятися даних, не боятися програмування, CLI та розвинути інфографічний смак

[Робочий щоденник курсу](https://public.etherpad-mozilla.org/p/uku2019)

[Домашні завдання](homeworks.md)



### День 1

### Вступний блок
11:40-13:00, 13:30-14:50, 15:00-16:20

- Про що цей курс. [Іл. 1](../vis/lections/figures/week01/fig_01.1.png) vs [Іл. 2](../vis/lections/figures/week01/fig_01.2.png) 
- Що відбувається у світі? (Texty. [The Pudding](https://pudding.cool/)). Як слідкувати за найкращим? Список конкурсів([1](https://www.informationisbeautifulawards.com/news/323-information-is-beautiful-awards-2018-the-winners), [2](http://www.malofiejgraphics.com/awards-list/), [3](https://datajournalismawards.org/2019/02/07/5-years-of-winning-data-journalism/), [4](https://www.snd.org/2019/02/2019-best-of-digital-medal-winners/) )  + твітер ([1](https://twitter.com/arnicas), [2](https://twitter.com/visualisingdata))
- Настрій цього курсу (морозиво і машина (ДЗ: чи це правда?) - пошук таємниць і відкриттів == розуміння світу)
- Для чого візуалізація? Приклади: [WSJ-вакцини](./img/vaccines.png), номери машин
- Історії, які ми шукаємо у даних ([Вонегут](https://www.youtube.com/watch?v=oP3c1h8v2ZQ), [презентація на LMF2017](https://docs.google.com/presentation/d/1_qLXvQYmdcdRsAq8wAFLxIvwnIrk5OrveEgACKQr0jo/edit#slide=id.g2255d7c6ec_1_110)) (найкращі - синтетичні проекти, подружіться з CompSci з УКУ!) 
- Великий цикл перероджень: дані-обробка-аналіз-візуалізація-дані-обробка-...
- Ефективна робота з інформацією, все зводиться до неї: [пошук](https://ahrefs.com/blog/google-advanced-search-operators/) + shortcuts, дві найкраші речі, про які ви тут дізнаєтесь  
- Як будувати роботу і вибирати тему
- Головна ідея візуалізації, наратив, історія. Що будем показувати? 
- Питання, які ви ставите до даних, і питання які вони  ставлять до вас 
- Особливості візуального сприйняття: Око і мозок, когнітивні особливості – звідки беруться принципи ефективної подачі - інформації. Як правильно кодувати інформацію у візуальну форму. (читання: William Cleveland, Visualizing data. Alberto Cairo, Stephen Few, Edward Tufty, etc)
- Пам'ять проти погляду. Salience. Pop-ups
- Мнемонічні правила інфодизайну. Далі - самі (див [курс на Прометеус](https://courses.prometheus.org.ua/courses/IRF/DV101/2016_T3/about) ) 
- Архітектура візуалізації (найважливіше - показуй найголовніше -> [ієрархія](https://www.canva.com/learn/typeface-fonts/) ) [відео](https://vimeo.com/13418563)
- Ще раз про важливість ієрархії: [приклад 1](https://www.ics.com/blog/and-winner-isthe-miss-universe-bad-design), [приклад 2](https://thehustle.co/steve-harvey-was-set-up-to-fail-in-miss-universe)
- [Шрифтовий дизайн](https://www.pierrickcalvez.com/journal/a-five-minutes-guide-to-better-typography) - з нього все починається, він - основа. [Книжка](https://practicaltypography.com/index.html)
- [Відео, графік, Darkhorse](https://www.youtube.com/watch?v=bDbJBWvonVI). Яке ДЗ на цей блок: 1. Знайти і передивитися всі відео від Darkhorse: [мапа](https://www.darkhorseanalytics.com/blog/data-looks-better-naked-maps-edition), [таблиця](https://www.darkhorseanalytics.com/blog/clear-off-the-table), [стовпчики](https://www.darkhorseanalytics.com/blog/data-looks-better-naked), [млинець](https://www.darkhorseanalytics.com/blog/salvaging-the-pie)

ДЗ: інсталяція [R](https://www.r-project.org/) та [RStudio](https://www.rstudio.com/products/rstudio/download/)
   
   
   
### День 2

### Перший інструмент: ChartBuilder. 
   - Табличні дані. Типи і формати даних ([csv](https://github.com/texty/president_polls/blob/master/data/chart_data_points.csv), [json - API](http://www.json.org/example.html), shp). [Широкий і довгий формат](https://docs.google.com/spreadsheets/d/1SCzjlPovSCJiJDlLgvM_EycM5BtN9LdQqnPWDPPyBog/edit#gid=0), який і для чого використовується?
   - Хором [робимо графіки](https://quartz.github.io/Chartbuilder/) 
   - Проблеми, які зустрічаються одразу (форматування, локалі, неправильна форма даних, ... - приклади.
   - Заводимо персональний github, робимо перший сайт на github.io


ДЗ: подивитися на [книгу](https://serialmentor.com/dataviz/)  



    
### Джерела даних: Інформаційні запити, Відкриті API, створюємо дані власноруч (приклади)

1. Інформаційні запити
2. OSINT, [Bellingcat's Digital Toolkit](https://docs.google.com/document/d/1BfLPJpRtyq4RFtHJoNpvWQjmGnyVkfE2HYoICKOGguA/edit)
3. Веб-Скрейпінг: Практичний воркшоп 
        - Як влаштована сторінка HTML (хором редагуємо сайт) 
        - Що таке теги, дерево елементів DOM, css, [css-selectors](https://www.w3.org/TR/css-2010/#selectors)
        - Знайомство з інструментами розробника
        - Перша програма на R (rvest)
   
4. Створити дані самому (зважуватися протягом року). 
5. Хороший [стиль, книга](http://worldpece.org/sites/default/files/datastyle.pdf) для роботи з даними. 
[Розуміння даних](https://exposingtheinvisible.org/guides/decoding-data/). 



------------ перші два дні насправді закінчили ся тут --------------------

ДЗ: завести API key для twitter  

### Дослідницький аналіз даних ([електронні таблиці](https://docs.google.com/spreadsheets/d/1yyMQ9BawYo-eR0kybB6-joeKE9SB8y2FL-OYoAP4kJU/edit?usp=sharing)). 
   - Сортування, фільтрація. Умовне форматування.
   - Робота з строковими функціями. 
   - Обчислення нових змінних(Трансформація значень у колонках). 
   - Групування та агрегація (pivot table).
   - Злиття таблиць(?)
   - Регулярні вирази - знайомство. Синтаксис. Застосування в електронних таблицях. TODO: notebook по регвиразам ((Бонус???))
   - РОбота з API через таблицю (((Бонус???)))

------------ перші два дні мали закінчитися тут --------------------


### День 3

-- 3 день

### Основні концепції програмування на прикладі Excel:
   - Змінні - це комірки. Трансформуємо дані у інші дані, за допомогою функцій 
   (числові, строкові тощо). - Що таке функція (гра у функції)
  
### Програмування у R - основні поняття
   - мотивація [82 річна японська пані](https://www.aarp.org/work/working-at-50-plus/info-2018/worlds-oldest-app-developer-fd.html)
   - для чого програмувати? Щоб була можливість менше працювати. Список нудних задач (((???)))
     (для прикладу, використовуємо роботу з Twitter API (скачаємо чиїсь твіти, наприклад))
   - середовище (пакети, завантаження даних, тощо)
   - Синтаксис: змінна, вектор, список, датафрейм, функція
   - векторизація (((можливо пізніше, на іншому прикладі)))
   - цикли
   - Ще раз, чому програмувати в R? [Excel vs R](https://www.jessesadler.com/post/excel-vs-r/) 


### День 4


### На рівень вище: Граматика даних
   - Добре структуровані дані
   - tidyverse 
   - Основні дієслова для роботи з даними
   - Pivot table за допомогою dplyr
   (Спочатку лише таблиці як результат, графіки - пізніше)



## День 5
-- 5 день
### Граматика графіки (практичний workshop)
   - анатомія ggplot та побудова графіків, 
   - Функції візуалізації даних. Які типи графіків використовувати у різних ситуаціях з різними типами даних. Ефективні види графіків, які нечасто використовуються: графік розсіяння, slope chart, dot chart, small multiples, гістограма

        -- Пропорції (співвідношення) 
        -- Динаміка
        -- Зв"язок
        -- Розподіл (+ пара необхідних термінів із статистики)
    - Екзотичні способи, [ксенографікс](https://xeno.graphics/)




ДЗ: [Книжка](http://socviz.co/) - Перегляньте 1 та 2, та обов'язково!!! прочитайте і повторіть всі приклади з кодом з 3, 4, 5 глави (вам потрібно буде близько 6 годин на це все)

[інша книжка: R for data sciense](https://r4ds.had.co.nz/index.html) - За бажанням, прочитайте дві глави, Data transformation та Data visualization



### Приклади дослідження даних 
   - що шукаємо?
   - case 1 [євробляхи](http://texty.org.ua/d/auto_euro/) (TODO: reproducible)
   - case 2, [diamonds](https://github.com/devrand/slides/blob/master/pdf26092017/diamonds_are_forever.Rmd)
   - case 3, ... літаки + самостійна робота
    
  
 ### Огляд інструментів для роботи з даними та візуалізацій
    - MOAL: http://bit.ly/12uokPm  
    - Raw (https://rawgraphs.io/)
    - Datawrapper (https://www.datawrapper.de/)
    
    - Vega / Vega Lite (https://vega.github.io/vega-lite/)
    - Idyll (http://idyll-lang.org/)
    - Floorish (https://flourish.studio/)
    
    - Observable (https://beta.observablehq.com/)
    - R/Python notebooks

    - Tableau (https://www.tableau.com/)  
    - Трохи застарілий, але корисний великий [список інструментів та джерел даних](https://docs.google.com/spreadsheets/d/1miN1dUvPMmnLdhunhZCil80LwlJ3xj8gRXrUNA-KrIE/edit#gid=0)

### Робота з кольором
- [гайд по інструментам](https://lisacharlotterost.github.io/2016/04/22/Colors-for-DataVis/)

### Перший великий проект. 
   
   - Вибір теми при наявному наборі даних( пробуємо використати "Як будувати роботу і вибирати тему")
   - Головні питання:
     -- яким є набір даних, які дані є, в якому стані. ( трохи пізніше: які інші можливі набори варто використати )?
     -- розуміння, чому ця візуалізація важлива. як визначати успіх? (навіщо вона, що хочеш досягнути, хто аудиторія, як будуть її використовувати)
     -- які обмеження?
     -- чи робили щось схоже?
      -- не всі рішення можна прийняти завчасно
      -- Дані можуть змінити початкові варіанти
      -- Читачі можуть змінити початкові варіанти
    ((Дати приклад такого конкретного аналізу))

- [список для перевірки](http://stephanieevergreen.com/dataviz-checklist/) 

------------- других три дні закінчуються тут --------------


## День 6

### Картографія. Статичні та інтерактивні карти на R
    - Приклади – типи карт. Формати даних, картографічна інформація, OSM 
    - Що таке GIS (приклад інтерфейсу, QGIS). 
    - Статична карта 
    - Та ж сама, але інтерактивна
        - Інтерактивні карти - анатомія. Гео-кодування 
        - Онлайн-сервіси: Carto, Mapbox
    - Коли не потрібно робити карти? 


### Відтворювана журналістика
    - RMarkdown
    - Інтерактивні візуалізації в R
    - Текст + Дані + Код
    - "Золоті"" принципи організації роботи з даними


### Консультаційна сесія: підготовка до фінального проекту

Практичні питання
Де взяти __ ?
    - SVG? (веб, crowbar) 
    - іконки?
    - мапки?
    - шрифти?

Куди рухатися далі? 
    - В напрямку постійної практики (мотиваційна промова)



***

### Оцінка результатів

    Якщо ви хоча б частково ходили на заняття і намагалися робити поточні завдання, це 60 балів
    За перше велике завдання (після березневих лекцій) - максимальна оцінка: 17 балів
    За друге велике завдання (фінальний проект)  - максимальна оцінка: 23 бали 
