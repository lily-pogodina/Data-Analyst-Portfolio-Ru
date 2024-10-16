# Анализ бизнес показателей развлекательного приложения.
<p align="center"><a href="https://github.com/lily-pogodina/Data-Analyst-Portfolio-Ru/blob/main/app_performance_analysis_ru/app_performance_analysis_ru.ipynb"><b>Открыть проект</b></a></p>

В ходе проекта мы рассмотрем несколько наборов данных, содержащих информацию о пользователях и их действиях, а также рекламных расходов развлекательного приложения Procrastinate Pro+. Несмотря на огромные вложения в рекламу, последние несколько месяцев компания терпит убытки. Наша задача — разобраться в причинах и помочь компании выйти в плюс.

**`Цели исследования**`**

* расcчитать прибыльность каждого клиента и в разбивке на категории
* выяснить окупаемость рекламы и стоимость привлечений клиентов по категориям
* уточнить убыточные когорты и разобраться в причинах убытков
* выяснить, в какие категории вложить рекламный бюджет

**`Итоги исследовательского анализа:`**

* Самое большое количество пользователей из США, также в США самая высокая доля платящих пользователей
* Самое большое количество пользователей iPhone, а вот самая доля платящих пользователей — у Mac (правда iPhone не сильно ниже) 
* Самое большое количество пользователей пришло органически, а ним идут пришедшие FaceBoom
* при этом самая большая доля платящих пользователей — у FaceBoom, а из пришедших органически пользователей, покупателей — всего 2%

Мы изучили расходы на маркетинг в распределении по рекламным источникам и сделали следующие наблюдения:

* Больше всего денег потратили на привлечение пользователей через TipTop (54751.30) и FaceBoom (32445.60)
* Расходы на маркетинг стабильно росли в течении наблюдаемого периода для TipTop (54751.30) и FaceBoom (32445.60) и достигли пика в сентябре. В октябре траты немного снизились. При этом для остальных источников вложения в маркетинг оставались стабильными и не превышали ≈1000 в месяц
* Самый высокий CAC опять TipTop, за ним следует FaceBoom. Учитывая, что именно в маркетинг на TipTop и FaceBoom мы тратим самое большое количество денег, стоит взглянуть на окупаемость этих источников (ROI).

Мы обнаружили ряд когорт, для которых реклама плохо окупается, при этом из исследовательского этапа мы знаем, что именно в этих когортах (США, TopTop, iPhone) у нас большая часть пользователей и высокие доли платящих пользователей. Для убыточных когорты предположили причины убыточности:

* **Пользователи из США.** Несмотря на то, что самое  большое количество пользователей из США, а также в США самая высокая доля платящих пользователей и высокая конверсия, у этой когорты низкое удержание и очень высокая стоимость привлечения новых пользователей
* **Пользователи, привлеченные через каналы TipTop, AdNonSense и FaceBoom:** конверсии у этих когорт в норме, но у AdNonSense и FaceBoom - очень плохое удержание (TipTop удержание нормальное), также у TipTop за исследуемый период резко выросла стоимость привлечения CAC, а у AdNonSense и FaceBoom они стабильно находятся на высоком уровне.
* **Пользователи устройств Mac, iPhone и Android:** Мы выяснили, что удержание и конверсия у пользователей этих устройств похожи, при этом у окупающегося PC даже ниже, чем у этих когорт. Скорее всего причина убыточности в высоком CAC.

**`Рекомендации для отдела маркетинга`**
* снизить вложения в маркетинг для устройств — Mac, Android и iPhone, стран — США, площадок — TipTop, AdNonSense и FaceBoom.
* перераспределить бюджет на рекламу, выделив прибыльные когорты, в нашем случае это пользователи PC, жители Великобритании. Для рекламы можно выделить канал lambdaMediaAds, у него хорошая и стабильная окупаемость и доля платящих пользователей.	
* уточнить у разработчиков, нет ли технических ошибок, которые бы повлияли на удержание клиентов убыточных когорт. Если такие ошибки есть и их устранить, то есть возможность поднять окупаемость.

 ---
 
**`Инструменты`**

* Python
  * pandas
  * matplotlib 
  * seaborn
  * предобработка
* исследовательский анализ
* визуализация

<p align="center"><a href="https://github.com/lily-pogodina/Data-Analyst-Portfolio-Ru"><b>К списку проектов</b></a></p>
