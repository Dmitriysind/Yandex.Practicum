# Поиск изображения по запросу

## Данные

В наличии были следующие данные:

- датасет изображений и запросов для тренировки модели
- датасет изображений и запросов для тестирование модели

Таблицы CrowdAnnotations и ExpertAnnotations с оценками соотношения запроса и изображения:

    - имя файла изображения
    - идентификатор описания
    - доля людей, подтвердивших, что описание соответствует изображению
    - количество человек, подтвердивших, что описание соответствует изображени
    - количество человек, подтвердивших, что описание не соответствует изображению

## Описание

Разработать модель, соединяющую текстовые данные и изображения. Сделать фильтр, исключащий из запроса тексты и изображение, содержащие детей

## Используемые библиотеки

`pandas`, `numpy`, `matplotlib`, `sklearn`, `keras`, `sentence_transformers`, `PIL`, `CLIP`
