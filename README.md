# Домашнее задание к лекции 7 «Асинхронность» 

## Решения
 * <a href="https://github.com/Nephedov/bjs-2-homeworks/blob/bjs-53/7.async/task.js">task.js</a> - код с реализованными функциями.

<a href="https://github.com/Nephedov/bjs-2-homeworks/tree/bjs-53/7.async">Репозиторий</a> с заданием и тестами.
Запуск через <a href="https://github.com/Nephedov/bjs-2-homeworks/blob/bjs-53/7.async/index.html">index.html</a>.

## Что было сделано
* Написан класс AlarmClock, в котором реализовано:
  * Метод добавления "звонка" в коллекцию:
    * Принимающий значение времени, функцию колбэка.
    * Генерирующий ошибку при отсутсвии какого-либо из аргументов.
    * Выводящий предупреждение в консоль о наличии такого же "звонка" в коллекции.
    * Поднимающий флаг возможности вызова "звонка" до совпадения времени "звонка" с текущим.
  * Метод удаления звонка по времени.
  * Метод сброса возможности вызова всех "звонков".
  * Метод удаления всех звонков и остановки интервала.
  * Метод start():
    * Проверяющий поднят ли флаг запущенного интервала.
    * Запускающий интервал в случае опущенного флага.
    * Вызывающий колбэк "звонка" в случае совпадения текущего времени со временем "звонка".
  * Метод stop() сбрасывающий интервал.
* Решение задания опубликовано в Github Pages.

## Описание Задания 1. Будильник-колыбельная

Помогите Васе перестать просыпать на пары. 
Для этого нужно написать программу-будильник-колыбельную с возможностью добавления, удаления, запусков и остановки звонков.
