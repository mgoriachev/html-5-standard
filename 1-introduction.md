# Глава 1. Введение

Рассказывается небольшая история стандарта. Данная глава НЕ является нормативной.

Раздел: **Serializability of script execution**
  - ***API*** ***HTML*** и ***DOM*** спроектированы для синхронного выполнения скриптов. Даже для ***worker*** поведение реализаций можно было рассматривать как полную сериализацию(*) выполнения всех сценариев
во всех глобальных переменных.
  - Исключением является ***SharedArrayBuffer***. Скрипты выполняются в агентах(*) фактически одновременно. Из-за модели памяти JavaScript существуют ситуации, которые не только невозможно
представить посредством - сериализованного выполнения сценариев, но также невозможно представить посредством сериализованного выполнения операторов среди этих сценариев.


### Пояснения
- **Сериализация** <<<нужно определение>>>
- **Агент** <<<Перенести определение из ECMA>>>
