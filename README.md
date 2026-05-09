# Titanic ML — Базовая классификация

Учебный проект: предсказание выживания пассажиров Титаника на основе пола, возраста, класса билета и других признаков.

## Что внутри

- **EDA** с pandas — анализ структуры данных и пропусков
- **Очистка данных**: median для age, mode для embarked, удаление утечки таргета
- **Feature Engineering**: One-Hot Encoding категориальных признаков
- **Logistic Regression** с stratified train/test split
- **Анализ Feature Importance** через коэффициенты модели

## Результаты

| Метрика | Значение |
|---------|----------|
| Accuracy | ~0.80 |
| Baseline (все умерли) | 0.62 |

**Главные предикторы выживания:**
1. Пол (женщины выживали чаще)
2. Класс билета (1-й класс выше шансы)
3. Возраст (моложе — выше шансы)

## Стек

`Python` `pandas` `scikit-learn` `seaborn` `matplotlib`

## Запуск

```bash
pip install pandas seaborn scikit-learn matplotlib
jupyter notebook titanic_ml.ipynb
```
