# Практическое занятие №3-4 — логистическая регрессия / классификация

Дисциплина «Алгоритмы машинного обучения для решения прикладных задач», семестр 1, МИРЭА.

Задание: [tasks/Практическое занятие №3-4.pdf](https://github.com/Mastertuz/ALM/blob/main/tasks/Практическое%20занятие%20№3-4.pdf) (файл хранится в ветке `main`).

## Содержимое ветки

- [solutions/pr2/Текущий контроль 2.ipynb](solutions/pr2/Текущий%20контроль%202.ipynb) — решение: бинарная классификация вин (`winequality-red.csv`) на "Хорошее" (`quality >= 7`) и "Не качественное" логистической регрессией: разбиение train/test, уравнение разделяющей гиперплоскости, классификация неизвестных вин, Accuracy / Precision / Recall, confusion matrix.
- [solutions/pr2/winequality-red.csv](solutions/pr2/winequality-red.csv) — исходные данные.
- [solutions/pr2/requirements.txt](solutions/pr2/requirements.txt) — зависимости для запуска в Google Colab.

## Итог

На тестовой выборке (25%, 400 вин): Accuracy = 0.845, Precision = 0.395, Recall = 0.278 (класс "Хорошее"). Из-за дисбаланса классов (~14% хороших вин) Recall низкий; с `class_weight='balanced'` Recall = 0.667 ценой падения Precision (0.336) и Accuracy (0.778). Подробности и confusion matrix — в ноутбуке.
