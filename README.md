<div align="center">
Министерство науки и высшего образования Российской Федерации <br />
Федеральное государственное бюджетное образовательное учреждение <br />
высшего образования <br />
«Московский государственный технический университет <br />
имени Н.Э. Баумана <br />
(национальный исследовательский университет)» <br />
(МГТУ им. Н.Э. Баумана)
</div>
<hr />
<div align="center">
ФАКУЛЬТЕТ ИНФОРМАТИКА И СИСТЕМЫ УПРАВЛЕНИЯ <br />
КАФЕДРА КОМПЬЮТЕРНЫЕ СИСТЕМЫ И СЕТИ (ИУ6)
</div>
<br />
<div align="center">
ОТЧЕТ <br />
по домашнему заданию <br />
по дисциплине "Современные средства разработки <br />
программного обеспечения"
</div>
<br />

Преподаватель: Фетисов М.В.

Студент группы ИУ6-54Б Каташинский Кирилл Юрьевич.

## Описание задания

Задача №10: "Коллекция монет".

Карточка Exhibit должна содержать следующие данные:

* специальное наименование (если есть);
* тип металла (перечисляемый тип);
* наименование валюты;
* количество единиц валюты;
* количество монет в коллекции

## Цели работы

На примере программы на языке С++:

* изучить объекты с разными видами состояний;
* определить инвариант класса;
* освоить работу с обобщёнными контейнерами стандартной библиотеки С++
* освоить работу с потоками ввода / вывода стандартной библиотеки С++
* освоить использование основных паттернов объектно-ориентированного проектирования
* освоить применение инструментов git и GitLab

## Адрес проекта

Проект хранится в репозитории по адресу: [https://bmstu.codes/lsx/mstd/iu6-5-2021/iu6-54b-kykatashinskiy/hw](https://bmstu.codes/lsx/mstd/iu6-5-2021/iu6-54b-kykatashinskiy/hw).

Описание классов хранится в репозитории по адресу: [http://lsx.pages.bmstu.codes/mstd/iu6-5-2021/iu6-54b-kykatashinskiy/hw/](http://lsx.pages.bmstu.codes/mstd/iu6-5-2021/iu6-54b-kykatashinskiy/hw/).

## Инвариант класса Exhibit

```cpp
bool invariant() const
{
    return _special_name.size() <= MAX_STRING_LENGTH && _metal_type >= RARE && _metal_type <= LIGHT &&
           _currency_name.size() <= MAX_STRING_LENGTH && _count_of_currency >= 0 && _count_of_coins >= 0;
}
```

## Выводы

В ходе данного домашнего задания была разработана программа для управления сохраняемой в файл коллекцией карточек заданного вида. Также была изучена работа с внешним репозиторием кода и сценарием непрерывной интергации.
