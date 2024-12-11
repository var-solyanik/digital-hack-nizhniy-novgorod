# Цифровой прорыв г. Нижний-Новгород. Сегментация водной поверхности по мультиспектральным снимкам. Анализ наводнений.

Проект решает проблему анализа водной поверхности на мультиспектральных спутниковых снимках. С помощью нашей модели есть возможность анализировать последствия наводнений. Кейс от СколТеха.

## Установка и запуск проекта
В файле requirements.txt указаны все нужные зависимости. Для работы также нужен Python ~3.10. Мы предоставили файлы fit.py для обучения модели на основе данных (их к сожалению предоставить не разрешили) и inference.py для предсказания на основе данных.

## Основной функционал проекта
Основной функционал - предсказание маски водной поверхности на основе мультиспектральных спутниковых снимков. Также был предоставлен функционал для обучения модели на основе предоставленных данных.

## Технологии и инструменты
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)

## Команда проекта
![Душенев Даниил](https://github.com/daniil-dushenev) - ML-engineer, разработка пайплайна обучения и инференса модели

![Карпов Назарий](https://github.com/nazar-karpov) - ML-engineer, разработка пайплайна обучения и инференса модели

![Зиновьев Даниил](https://github.com/Tanjiro00) - ML-engineer, разработка пайплайна обучения и инференса модели

![Соляник Варвара](https://github.com/var-solyanik) - ML-engineer, исследования и добавление фичей в инференс

![Луценко Александра](https://github.com/Lutsenko12) - ML-engineer, исследования и добавление фичей в инференс

## Структура проекта
#### dataset.py
Модуль для предобработки и работы с набором данных спутниковых изображений и масок

#### fit.py
Этот скрипт предназначен для обучения модели сегментации (например, UNet++) на наборе данных изображений и их масок, включая различные функции предобработки и методику логирования метрик.

#### inference.py
Этот скрипт выполняет предсказание масок для крупных спутниковых снимков с использованием обученной модели UNet++ и PyTorch.

## Демонстрация работы прототипа
![изображение](https://github.com/user-attachments/assets/d7683f08-8e56-4e18-8a7a-171006bc0f91)

## Заключение
Наш проект имеет ценность для анализа последствий наводнений. Определение затопленных территорий с использованием данных дистанционного зондирования Земли (ДЗЗ) является важной задачей экологического мониторинга. Паводки наносят значительный экономический ущерб, и автоматизация процесса их распознавания с помощью ИИ позволяет оперативно анализировать обширные территории, что критично для принятия решений. Важность использования мультиспектральных спутниковых данных заключается в возможности точного распознавания водных поверхностей и оценки пострадавших объектов инфраструктуры. Наша модель с хорошей точностью определяет, где на поверхности находится вода.

## Лицензия Apache

