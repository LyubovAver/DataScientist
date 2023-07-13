# DataScientist
Проекты, выполненные в процессе обучения по направлению "Специалист по Data Science"
## Проект 1
Сравнение Москвы и Петербурга окружено мифами. 
На данных Яндекс Музыки вы сравним поведение пользователей двух столиц.

Цель исследования — проверить три гипотезы:

    1.Активность пользователей зависит от дня недели. Причём в Москве и Петербурге это проявляется по-разному.
    2.В понедельник утром в Москве преобладают одни жанры, а в Петербурге — другие. Так же и вечером пятницы преобладают разные жанры — в зависимости от города.
    3.Москва и Петербург предпочитают разные жанры музыки. В Москве чаще слушают поп-музыку, в Петербурге — русский рэп.

Ход исследования

Данные о поведении пользователей получим из файла yandex_music_project.csv. О качестве данных ничего не известно. Поэтому перед проверкой гипотез понадобится обзор данных.
Проверим данные на ошибки и оцениим их влияние на исследование. Затем, на этапе предобработки поищем возможность исправить самые критичные ошибки данных.

Таким образом, исследование пройдёт в три этапа:

    1.Обзор данных.
    2.Предобработка данных.
    3.Проверка гипотез.
Использована библиотека pandas

## Проект 2. Исследование надежности заемщиков
Описание проекта
Заказчик — кредитный отдел банка. Нужно разобраться, влияет ли семейное положение и количество детей клиента на факт погашения кредита в срок. Входные данные от банка — статистика о платёжеспособности клиентов.
Результаты исследования будут учтены при построении модели кредитного скоринга — специальной системы, которая оценивает способность потенциального заёмщика вернуть кредит банку.
Описание данных

    children — количество детей в семье
    days_employed — общий трудовой стаж в днях
    dob_years — возраст клиента в годах
    education — уровень образования клиента
    education_id — идентификатор уровня образования
    family_status — семейное положение
    family_status_id — идентификатор семейного положения
    gender — пол клиента
    income_type — тип занятости
    debt — имел ли задолженность по возврату кредитов
    total_income — ежемесячный доход
    purpose — цель получения кредита
Использована библиотека pandas

## Проект 3. Исследование объявлений о продаже квартир
Описание проекта
В вашем распоряжении данные сервиса Яндекс Недвижимость — архив объявлений за несколько лет о продаже квартир в Санкт-Петербурге и соседних населённых пунктах.
Ваша задача — выполнить предобработку данных и изучить их, чтобы найти интересные особенности и зависимости, которые существуют на рынке недвижимости.
О каждой квартире в базе содержится два типа данных: добавленные пользователем и картографические. Например, к первому типу относятся площадь квартиры, её этаж и количество балконов, ко второму — расстояния до центра города, аэропорта и ближайшего парка.
Использованы библиотеки: pandas,datetime,numpy,seaborn

## Проект 4.
Описание проекта
Вы аналитик компании «Мегалайн» — федерального оператора сотовой связи. Клиентам предлагают два тарифных плана: «Смарт» и «Ультра». Чтобы скорректировать рекламный бюджет, коммерческий департамент хочет понять, какой тариф приносит больше денег.
Вам предстоит сделать предварительный анализ тарифов на небольшой выборке клиентов. В вашем распоряжении данные 500 пользователей «Мегалайна»: кто они, откуда, каким тарифом пользуются, сколько звонков и сообщений каждый отправил за 2018-й год. Нужно проанализировать поведение клиентов и сделать вывод — какой тариф лучше.
Использованы библиотеки pandas,numpy,seaborn,matplotlib,scipy

# Сборный проект. 
 Общий вывод

В процессе изучения датасета с информацией об игровых платформам в разрезе разных стран и лет для прогнозирования тактики поведения на 2017 год были получены следующие выводы:

   1. На графике распределения продаж платформ по годам, можно проследить закономерность, что примерный "срок жизни" платформы около 10 лет, на 5-6 году жизни платформа достигает пика продаж. Из всех платформ с максимальными продажами только PC существует около 30 лет, но продажи равномерны, без взлётов. Новые платформы появляются практически ежегодно.

   2.Для построения прогноза на 2017 год были взяты данные за предыдущие 3 года:2014,2015 и 2016.

   3.  По гистограмме распределения изменения продаж по платформам в 2014-2016 гг. видно, что лидерами по общему количеству проданных копий являются 4 (более 50 млн.) плтаформы:"3DS","XOne","PS4","PS3"

  4.  На графике зависимости суммарных продаж по годам выпуска продажи по всем платформам стремятся на понижение. Если не заглядывать далеко в будущее, то большую прибыль пока дают и будут давать в 2017 году платвформы XOne и PS4, но не известно в течении какого срока. Также есть платформы со стабильными продажами, без резких подъемов и спусков, такие как 3DS,PC,PSV. Возможно их продажи и дальше будут приносить стабильную, но небольшую прибыль.

  5.  Для отдельного изучения была выбрана платформа PS4, мы видим прямую связь продаж с оценками критиков и обратную с оценками пользователей, пусть и не очень большую. Можно сделать вывод, что любой пиар - хороший или плохой идет на пользу продажам.

  6.  Наиболее распространенный жанр игр - Action, к наиболее продаваемым относятся - Action и Shooter. По диаграммам размаха видно, что каждый показатель имеет много выбросов, есть перекосы и распределение неравномерное.

   7. Во всех странах, кроме Японии в лидерах оказались PS4 и XOne. В Северной Америке и Европе достаточно большие продажи игр, в Японии и других странах несколько ниже, да и вообще картина популярных платформ в Японии отличается от всего мира.

  8.  Среди популярных жанров во всех странах, кроме Японии преобладает Action, Shooter,Sports. В Японии к жанру Action ддобавились Role-playing и Fighting. Из всего вышесказанного можно сделать вывод, что для всех стран кроме Японии стратегия развития игр привержена одним и тем же тенденциям.

  9.  Также были составлены портреты пользователей по разным странам. Все они примерно схожи, не считая Японии, игровая индустрия в ней идет по своему пути.

 10.   Проверены две гипотезы: Средние пользовательские рейтинги платформ Xbox One и PC одинаковые; Средние пользовательские рейтинги жанров Action (англ. «действие», экшен-игры) и Sports (англ. «спортивные соревнования») разные. Первую - не отвергли, вторую - отвергли



## Проект 5. Рекомендация тарифов
Описание проекта
Оператор мобильной связи «Мегалайн» выяснил: многие клиенты пользуются архивными тарифами. Они хотят построить систему, способную проанализировать поведение клиентов и предложить пользователям новый тариф: «Смарт» или «Ультра».
В вашем распоряжении данные о поведении клиентов, которые уже перешли на эти тарифы. Нужно построить модель для задачи классификации, которая выберет подходящий тариф. Предобработка данных не понадобится — вы её уже сделали.
Постройте модель с максимально большим значением accuracy. Чтобы сдать проект успешно, нужно довести долю правильных ответов по крайней мере до 0.75. Проверьте accuracy на тестовой выборке самостоятельно.
Дополнительно использована библиотека sklearn


## Проект 6. Отток клиентов
Из «Бета-Банка» стали уходить клиенты. Каждый месяц. Немного, но заметно. Банковские маркетологи посчитали: сохранять текущих клиентов дешевле, чем привлекать новых.
Нужно спрогнозировать, уйдёт клиент из банка в ближайшее время или нет. Вам предоставлены исторические данные о поведении клиентов и расторжении договоров с банком. 
Постройте модель с предельно большим значением F1-меры. Чтобы сдать проект успешно, нужно довести метрику до 0.59. Проверьте F1-меру на тестовой выборке самостоятельно.
Дополнительно измеряйте AUC-ROC, сравнивайте её значение с F1-мерой. 
Дополнительно используем классы из sklearn: LogisticRegression,RandomForestClassifier,StandardScaler,DecisionTreeClassifier,accuracy_score,
confusion_matrix,
recall_score,
precision_score,
f1_score,
roc_curve,
roc_auc_score

## Проект 7. Выбор локации для скважины

Допустим, вы работаете в добывающей компании «ГлавРосГосНефть». Нужно решить, где бурить новую скважину.

Вам предоставлены пробы нефти в трёх регионах: в каждом 10 000 месторождений, где измерили качество нефти и объём её запасов. Постройте модель машинного обучения, которая поможет определить регион, где добыча принесёт наибольшую прибыль. Проанализируйте возможную прибыль и риски техникой Bootstrap.

Шаги для выбора локации:

    1.В избранном регионе ищут месторождения, для каждого определяют значения признаков;
    2.Строят модель и оценивают объём запасов;
    3.Выбирают месторождения с самым высокими оценками значений. Количество месторождений зависит от бюджета компании и стоимости разработки одной скважины;
    4.Прибыль равна суммарной прибыли отобранных месторождений.
Дополнительно использована библиотека scipy

## Проект 8. Сборный проект. Восстановление золота из руды
Подготовьте прототип модели машинного обучения для «Цифры». Компания разрабатывает решения для эффективной работы промышленных предприятий.

Модель должна предсказать коэффициент восстановления золота из золотосодержащей руды. Используйте данные с параметрами добычи и очистки.

Модель поможет оптимизировать производство, чтобы не запускать предприятие с убыточными характеристиками.

Вам нужно:

    1.Подготовить данные;
    2.Провести исследовательский анализ данных;
    3.Построить и обучить модель.

Чтобы выполнить проект, обращайтесь к библиотекам pandas, matplotlib и sklearn. Вам поможет их документация.
