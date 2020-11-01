# Вопросы для собеседования на Java Software Test Automation Engineer

+ [ПРИНЦИПЫ ООП](#принципы-ооп)
+ [ПРИНЦИПЫ ООП (АББРЕВИАТУРЫ)](#принципы-ооп-аббревиатуры)
+ [ACCESS MODIFIERS](#access-modifiers)
+ [PATTERNS](#patterns)
+ [equals() VS "=="](#)
+ [Interface VS Abstract Class](#)
+ [PRIMITIVE TYPES](#)
+ [FLOAT VS DOUBLE](#)

# ПРИНЦИПЫ ООП

Абстракция (Abstaraction).
Выделение существенных характеристик объекта и пренебрежение незначительными к контексте решаемой задачи.

Инкапсуляция (Encapsulation).
Сокрытие реализации. Пример: это как машина с двумя педалями (тормоз, газ). Это как public методы для скрытой логики под капотом.

Наследование (Inheritance).
Наследуя класс, можно добавлять методы и свойства характерные только для наследника. В Java одиночное только, иначе Diamond Problem.

Полиморфизм (Polymorphism).
1 method name a lot of implementations. (@Override)
Interfaces: Metod implementation in each class can be customized.
Classes: Использование одного и того же имени метода в классах унаследованных от одного (абстрактного) суперкласса.

# ПРИНЦИПЫ ООП (АББРЕВИАТУРЫ)

S - Single Responsibility
O - Open/Closed
L - Liskov Substitution
I - Interface Segregation
D - Dependency Inversion

Single Responsibility - каждый объект должен иметь одну обязанность и она должна быть полностью инкапсулированная в класс, а все его сервисы должны быть напрвлены исключительно на обеспечение этой обязанности.

Open/Closed - software entities "программные сущности" (classes, modules, functions, etc.) открыты для расширения/закрыты для изменения. Поля private методы public(нужные).

Liskov Substitution - метод супер класса должен одинаково хорошо работать как с ним (супер классом) так и с его наследниками. Чтобы можно было методы параметризировать супер классом, а работать со всем достигая таким образом необходимого уровня абстракции.

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

# ACCESS MODIFIERS

![icon][ACCESS_MODIFIERS]

[ACCESS_MODIFIERS]:ACCESS_MODIFIERS.jpeg

# PATTERNS

![icon][PATTERNS]

[PATTERNS]:PATTERNS.png

![icon][Decorator]

[Decorator]:Decorator.png

![icon][Singleton_1]

[Singleton_1]:Singleton_1.png

![icon][Builder_1]

[Builder_1]:Builder_1.png

# equals() VS "=="

equals() - метод. Method for content comparison.
 "==" - оператор. Checks if both objects point to the same memory location.
 
# Interface VS Abstract Class
 
![icon][Interface_VS_Abstract_Class]

[Interface_VS_Abstract_Class]:Interface_VS_Abstract_Class.png
 
# PRIMITIVE TYPES
 
![icon][PRIMITIVE_TYPES]

[PRIMITIVE_TYPES]:PRIMITIVE_TYPES.png

 # FLOAT VS DOUBLE
 
 float 32 bits - double 64 bits
 7 знаков после запятой - 16 знаков после запятой
 https://javarush.ru/groups/posts/2136-ustroystvo-vejshestvennihkh-chisel

























































Tricky questions:
Можно ли создать объект абстрактного класса? - нет
Can interface extends class? - yes. how many - one
