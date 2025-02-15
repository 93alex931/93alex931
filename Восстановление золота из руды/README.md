# Восстановление золота

**Статус:** Завершён.

**Цель проекта:** Обучить модели, чтобы оптимизировать технологический процесс восстановления золота из руды.

**Результаты работы:**
   - Мы изучили имеющиеся данные, избавились от пропусков, **исправили ошибки** в выборках;
   - Проанализировали некоторые из признаков, чтобы **лучше понять технологический процесс** и выбрать значимые признаки для обучения моделей;
   - Предприняли попытку **обнаружения аномально низких значений** целевого признака при помощи модели-классификатора;
   - Обучили большое количество разных **моделей** для предсказания качества флотации и конечного качества восстановления по входным параметрам:
       - Выявили, какие модели и на каких наборах признаков дают **лучший результат**;
       - Взяли лучшие модели и **оптимизировали их гиперпараметры**, чтобы ещё больше улучшить качество предсказаний;
       - **Проверили** модели **на адекватность**, сравнив их точность с точностью случайной модели.
   - Выяснили, насколько хорошо модель для оценки финального качества восстановления **подбирает оптимальные параметры** для технологического процесса:
       - Выполнили *bootstrap*, чтобы **смоделировать ситуацию**, в которой мы можем сделать ограниченное число экспериментов;
       - С помощью модели мы достигли низкого значения **RMSE**,
       - в то время как качество по всей выборке без оптимизации имеет размах от *~50%* до *~80%* со средним в *70%*;
       - **Предложили усреднённые параметры технологического процесса**, выбранные моделью, и посчитали их потенциальную отдачу по формуле. Отдача получилась в диапазоне **RMSE 10-14**, что близко к максимальному известному значению.
   
---
