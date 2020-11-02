# Вопросы для собеседования на Java Software Test Automation Engineer

+ [ПРИНЦИПЫ ООП](#принципы-ооп)
+ [ПРИНЦИПЫ ООП (АББРЕВИАТУРЫ)](#принципы-ооп-аббревиатуры)
+ [ACCESS MODIFIERS](#access-modifiers)
+ [PATTERNS](#patterns)
+ [equals() VS "=="](#equals-vs-)
+ [Interface VS Abstract Class](#interface-vs-abstract-class)
+ [PRIMITIVE TYPES](#primitive-types)
+ [FLOAT VS DOUBLE](#float-vs-double)
+ [CI CD](#ci-cd)
+ [Version Control Systems](#version-control-systems)
+ [GIT advantages/disadvantages](#)
+ [Cognitive Complexity](#cognitive-complexity)
+ [Casting of objects in java](#casting-of-objects-in-java)

# ПРИНЦИПЫ ООП

Object Oriened Programming

• **Абстракция** (Abstaraction).
Выделение существенных характеристик объекта и пренебрежение незначительными к контексте решаемой задачи.

• **Инкапсуляция** (Encapsulation).
Сокрытие реализации. Пример: машина с двумя педалями (тормоз, газ). Это как public методы для скрытой логики под капотом. Обеспечивает защиту данных от прямого внешнего доступа и неправильного использования.

• **Наследование** (Inheritance).
Наследуя класс, можно добавлять методы и свойства характерные только для наследника. В Java одиночное только, иначе Diamond Problem.

• **Полиморфизм** (Polymorphism).
1 method name a lot of implementations. (**@Override**)

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

equals() - **метод**. Method for content comparison.

 "==" - **оператор**. Checks if both objects point to the same memory location.
 
# Interface VS Abstract Class
 
![icon][Interface_VS_Abstract_Class]

[Interface_VS_Abstract_Class]:Interface_VS_Abstract_Class.png
 
# PRIMITIVE TYPES
 
![icon][PRIMITIVE_TYPES]

[PRIMITIVE_TYPES]:PRIMITIVE_TYPES.png

# FLOAT VS DOUBLE

**float** 32 bits - **double** 64 bits

7 знаков после запятой - 16 знаков после запятой

https://javarush.ru/groups/posts/2136-ustroystvo-vejshestvennihkh-chisel

# CI CD
 
**CI** - Continious Integration

**The key goals of continuous integration are:**

**1.** Improve software quality: to find and address bugs quicker.

**2.** Reduce the time it takes to validate and release new software updates.

**CD** - Continious Delivery

![icon][CI]

[CI]:CI.png

# Version Control Systems

Solutions:

![icon][VCS_1]

[VCS_1]:VCS_1.png

**Lock-modify-unlock** (example: Excel file on server) - is a very simple solution. In such a system, the repository allows only one person to change a file at a time. First Harry must lock the file before he can begin making changes to it. Locking a file is a lot like borrowing a book from the library; if Harry has locked a file, then Sally cannot make any changes to it. If she tries to lock the file, the repository will deny the request. All she can do is read the file, and wait for Harry to finish his changes and release his lock. After Harry unlocks the file, his turn is over, and now Sally can take her turn by locking and editing.

**Copy-modify-merge** model as an alternative to locking. In this model, each user's client reads the repository and creates a personal working copy of the file or project. Users then work in parallel, modifying their private copies. Finally, the private copies are merged together into a new, final version. The version control system often assists with the merging, but ultimately a human being is responsible for making it happen correctly.

https://tortoisesvn.net/docs/release/TortoiseSVN_en/tsvn-basics-versioning.html

![icon][VCS_2]

[VCS_2]:VCS_2.png

https://homes.cs.washington.edu/~mernst/advice/version-control.html

# GIT advantages/disadvantages
+ Distributed
+ Free and Open Source
+ The most popular --> Community --> Q&A

![icon][GIT_1]

[GIT_1]:GIT_1.png

https://git-scm.com/book/en/v2

https://www.softwaretestinghelp.com/version-control-software/

# Cognitive Complexity

![icon][Complexity]

[Complexity]:Complexity.png

https://www.sonarsource.com/docs/CognitiveComplexity.pdf

![icon][Complexity_1]

[Complexity_1]:Complexity_1.png
![icon][Complexity_2]

[Complexity_2]:Complexity_2.png
![icon][Complexity_3]

[Complexity_3]:Complexity_3.png

# Casting of objects in java

![icon][Cast]

[Cast]:Cast.jpeg






































# Tricky questions:
Можно ли создать объект абстрактного класса? - нет
Can interface extends class? - yes. how many - one
