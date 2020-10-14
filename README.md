# Project-idias
Модель универсального приведения парсинга к модели связей данных (XML), из слечения последовательностей/групп структур:
1я - представляет многосвязный список со связями групп данных:
1й последовательности ввода(дорожки данных),
2й соединения эквивалентных величин (возможные вариации),
3й составные эллементы груп или NILL(для элементарных связей).

2я - структуры связных списков отрожающих модели возможных вариаций групп(гипотизы).
1Я -повательностей вида (1..n).-> со счетчиком количества на участке.
2Я -повательностей вида (N..n).-> со счетчиком количества на участке.
3й - Группа вариантов гипотез для нахождение наиболее удачного сочетания.
(Данные структуры находятся в процессе отладки/разработки,тем немение ознакомится с частичной реализацией для лучшего понимания можно по ссылке https://github.com/AlexitScientist/java-struct-)
Принцип сличения данных по 2м принципам:
1я создание комбинаций (1..1 or 2..1 or 1..2) сличением вида проверки количества повторения последовательностей комбинаций данных a-b-c и 
a-b.
2я анализ совпадений последовательностей:
По принципу отношения групп множеств вида ( a-c, b-d) or (a-n, b-f),эквивалентно связям 1..n и n..n,
где a и b будут эквивалентом 1го участка эквивалентных данных исходя из равного количества повторений(принцип аналогии),
образуя между собой 1..1, при этом c-n и d-f формально будут несортированной кучей вида n..n. 
Построение баланса(определение оптимального набора) для формирования представления групп отношений систем при определении типа захвата(1-2 or 2-1) в виде дублирования модели гипотиз...
Данная разработка будет полезна для формирования групп  отношений в области автоматизации и проектирования систем.
Переводя множества к табличным отношениям (1..0, 1..1, 1..n, n..n).
Также данная модель может в дальнейшем служить реализацией транслятора языков(из 3х блоков) вида:
1й парсировалбы фаил входных параметров.(поля ввода) формируя граф контекста.(для проведения паралелий используемых операций)
2й парсировалбы файлов структуры библиотеки.(для однозначности последующего разделения блоков кода и описания функционала).
3й Парсинг документации, создающий входы между упоминанием процесса в древе представления вариаций содержащих описание и код.
(для создания соответствий вида  опесание-команда(1)->опесание-команда(2) ).
Таким образом проводя деление данных по принципу составления хмл древьев, на основе драбрения на таргеты методами  дробления и склейки совпадений вхождения.
(Реальность и предпосылки к реализации взяты из работ Машины Тьюринга,орм и ряда других работ)

