# Приоритизация гипотез и анализ A/B-теста для интернет-магазина
<p align="center"><a href="https://github.com/lily-pogodina/Data-Analyst-Portfolio-Ru/blob/main/A_B_testing_%26_hypothesis_prioritizing_for_e-commerce_ru/A_B_testing_%26_hypothesis_prioritizing_for_e-commerce_ru.ipynb"><b>Открыть проект</b></a></p>

В нашем распоряжении файлы, содержащие ряд гипотез для увеличения выручки, а также результаты A/B-теста.
\
В исследовании мы применим ряд фреймворков и выберем наиболее приоритетные гипотезы, а также проанализируем результаты A/B-теста.

**`Цели исследования**`**

* выяснить наиболее перспективную гипотезу
* проанализировать результаты A/B-теста и принять решение о продолжении теста или его остановки
* yзнать, есть ли значимая разница между группами `A` и `B`, на основе уже имеющихся данных

---
**`Приоритизация гипотез:`**

Применили два способа приоритизации гипотез RICE и ICE. 

* При применении способа ICE в топ 3 попали гипотезы №№ 8,0,7, с №8 на первом месте.
* После применения способа RICE на первое место по приоритетности вышла гипотеза №7
№8 ушла в середину списка, 0 остался в топ 3, также в топ 3 поднялась гипотеза под номером №2
(На изменение положения гипотез в шкале приоритетности повлиял параметр `reach` (англ. «охват»).)

**`Результаты A/B-теста`**

**Приняли решение: остановить тест, зафиксировать победу группы `B`.**

Основания для принятия решения мы получили на основе графиков, а так же расчета стат. значимости для среднего чека и средней суммы заказов между группами. Для расчета стат. значимости мы использовали как 'сырые', так и 'очищенные'
от аномалий данные. Дополнительно считали относительную разницу средних значений `B` к `А`

Выводы получились следующими:

* Есть значимое различие по среднему количеству заказов между группами как по «сырым», так и по данным после фильтрации аномалий. Разница между сегментами равна 16% для "сырых" и 20,5% для "очищенных" данных в пользу группы `B` 

* Нет статистически значимого различия по среднему чеку между группами ни по «сырым», ни по данным после фильтрации аномалий. Разница между сегментами равна 28,7% для "сырых" и 5.5% для "очищенных" данных в пользу группы `B` 

* График различия среднего количества заказов между группами сообщает, что результаты группы `B` стабильно лучше группы `А` на 10-20%

* График различия среднего чека между группами сообщает, что результаты группы `B` в конце и начале наблюдений  лучше группы `А`. Отношение (B/A-1) почти все время больше ноля (30% к концу наблюдений).

**`Рекомендации для отдела маркетинга`**

* Следует обратить внимание на гипотезу №7, как на наиболее приоритетную, а также обладающую наибольшим охватом (10 из 10 пунктов)

* Признать A/B-тест успешным и реализовать изменения, характерные для группы B

 ---
 
**`Инструменты`**

* Python
  * pandas
  * matplotlib 
  * seaborn
  * предобработка
* исследовательский анализ
* статистический анализ
* визуализация
* А/B тестирование

<p align="center"><a href="https://github.com/lily-pogodina/Data-Analyst-Portfolio-Ru"><b>К списку проектов</b></a></p>
