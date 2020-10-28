# Вопросы для собеседования на Java Software Test Automation Engineer

+ [ПРИНЦИПЫ ООП](#ПРИНЦИПЫ ООП)
+ [ПРИНЦИПЫ ООП (АББРЕВИАТУРЫ)](#ПРИНЦИПЫ ООП (АББРЕВИАТУРЫ))
+ [ACCESS MODIFIERS](#ACCESS MODIFIERS)

## ПРИНЦИПЫ ООП.
Абстракция (Abstaraction). Выделение существенных характеристик объекта и пренебрежение незначительными к контексте решаемой задачи.
Инкапсуляция (Encapsulation). Сокрытие реализации. Пример: это как машина с двумя педалями (тормоз, газ). Это как public методы для скрытой логики под капотом.
Наследование (Inheritance). Наследуя класс, можно добавлять методы и свойства характерные только для наследника. В Java одиночное только, иначе Diamond Problem.
Полиморфизм (Polymorphism). 1 metjod a lot of implementations(Interfaces). Использование одного и того же имени метода в различных объектах(обычно унаследованных от одного суперкласса).

## ПРИНЦИПЫ ООП (АББРЕВИАТУРЫ).

S - Single Responsibility
O - Open/Closed
L - Liskov Substitution
I - Interface Segregation
D - Dependency Inversion
Single Responsibility - каждый объект должен иметь одну обязанность и она должна быть полностью инкапсулированная в класс, а все его сервисы должны быть напрвлены исключительно на обеспечение это йобязанности.
Open/Closed - открыт для расширения/закрыт для изменения.Поля private методы public(нужные).
Liskov Substitution - метод супер класса одинаково хорошо работать с должен как с ним так и с его наследниками. Чтобы можно было методы параметризировать супер классом, а работать со всем достигая таким образом необходимого уровня абстракции.
Interface Segregation - больше интерфейсов лучше (имплементишь из них только столько сколько надо конкретному объекту), чем один с несколькими методами и потом думать о заглушках для нерелевантных для объекта методов.
Dependency Inversion - принцип инверсии зависимостей. Если есть возможность то завязываться на абстрактных классах и интерфейсах, чтобы модули программы не зависели от конкретных реализаций, а от абстракций.

D - Don't
R - Repeat
Y - Yourself
Избегайте повторного написания кода, вынося в абстракции часто используемые задачи и данные. Каждая часть вашего кода или информации должна находиться в единственном числе в единственном доступном месте. Это один из принципов читаемого кода.

K - Keep
I - It
S - Short/Small
S - Simple

Y - You
A - Aren't
G - Gonna
N - Need
I - It

## ACCESS MODIFIERS.

[1]:1.jpeg
