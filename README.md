# Выбор локации для скважины

Допустим, вы работаете в добывающей компании «ГлавРосГосНефть». Нужно решить, где бурить новую скважину.

Вам предоставлены пробы нефти в трёх регионах: в каждом 10 000 месторождений, где измерили качество нефти и объём её запасов. Постройте модель машинного обучения, которая поможет определить регион, где добыча принесёт наибольшую прибыль. Проанализируйте возможную прибыль и риски техникой  _Bootstrap._

**Шаги для выбора локации:**

-   В избранном регионе ищут месторождения, для каждого определяют значения признаков;
-   Строят модель и оценивают объём запасов;
-   Выбирают месторождения с самым высокими оценками значений. Количество месторождений зависит от бюджета компании и стоимости разработки одной скважины;
-   Прибыль равна суммарной прибыли отобранных месторождений.

**Данные геологоразведки трёх регионов:**

-   id — уникальный идентификатор скважины;
-   f0, f1, f2 — три признака точек;
-   product — объём запасов в скважине (тыс. баррелей).

**Цель данной работы**  - Построить модель, способную определить наиболее доходных регион добычи нефти.

**Работа пройдет в следующие 5 этапов:**

1.  Загрузка и подготовка данных;
2.  Обучение и проверка моделей;
3.  Подготовка к расчёту прибыли;
4.  Расчёт потенциальной прибыли;
5.  Расчёт рисков.

## Вывод

По резульатам работы, можно сказать, что наиболее оптимальным регионом является  `Регион 1`:

-   Потенциальная  `выручка`  от лучших 200 скважин 12415086.70, а  `прибыль`  - 2415086.70;
-   Потенциальный  `ROI`  от лучших 200 скважин 24.15%;
-   Потенциальные  `2.5% квантиль прибыли`  составляет 91700.57;
-   Потенциальный  `риск`, выраженный в прогнозируемой доли отрицательной прибыли, составляет 0.6%.

Таким образом, для бурения новых скважин рекомендуется использовать  `Регион 1`.
