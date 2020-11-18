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
+ [Преобразование типов](#преобразование-типов)
+ [Methods "Overload" VS @Override](#methods-overload-vs-override)
+ [Tricky questions](#tricky-questions)

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

[ACCESS_MODIFIERS]:ACCESS_MODIFIERS.png

https://www.javatpoint.com/access-modifiers

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
![icon][Interface_VS_Abstract_Class_1]

[Interface_VS_Abstract_Class_1]:Interface_VS_Abstract_Class.png

https://www.javatpoint.com/difference-between-abstract-class-and-interface
 
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

# Преобразование типов

В Java возможны 7 видов приведений:
+ тождественное (identity);
+ расширение примитивного типа (widening primitive);
+ сужение примитивного типа (narrowing primitive);
+ расширение объектного типа (widening reference);
+ сужение объектного типа (narrowing reference);
+ преобразование к строке (String);
+ запрещенные преобразования (forbidden).

![icon][identity]

[identity]:identity.png

Для простых типов расширение означает, что осуществляется переход от менее емкого типа к более емкому.
Например, от типа byte (длина 1 байт) к типу int (длина 4 байта).
Такие преобразования безопасны в том смысле, что новый тип всегда гарантированно вмещает в себя все данные,
которые хранились в старом типе, и таким образом не происходит потери данных. Именно поэтому компилятор осуществляет его сам (не явно).

![icon][wp]

[wp]:wp.png

Обратное преобразование - сужение - означает, что переход осуществляется от более емкого типа к менее емкому.
При таком преобразовании есть риск потерять данные. Например, если число типа int было больше 127,
то при приведении его к byte значения битов старше восьмого будут потеряны.
В Java такое преобразование должно совершаться явным образом, т.е. программист в коде должен явно указать,
что он намеревается осуществить такое преобразование и готов идти на потерю данных.

![icon][np]

[np]:np.png

![icon][np1]

[np1]:np1.png

![icon][np2]

[np2]:np2.png

![icon][np3]

[np3]:np3.png

Расширение объектного типа - означает переход от более конкретного типа к менее конкретному, т.е. переход от детей к родителям.
Подобно случаю с примитивными типами, этот переход производится самой JVM при необходимости и незаметен для разработчика,
то есть не требует никаких дополнительных усилий, так как он всегда успешен: всегда можно обращаться к объекту, порожденному от наследника, по типу его родителя.
Обращаем внимание, что при подобном преобразовании с самим объектом ничего не происходит.
Не смотря на то, что, например, поле y класса Child теперь больше не доступно, это не говорит о том, что оно исчезло.
Такое существенное изменение структуры объекта невозможно. Он был порожден от класса Child, и навсегда сохранит все его свойства.
Изменился лишь тип ссылки, через которую идет обращение к объекту.
Эту ситуацию можно условно сравнить с рассматриванием некоего предмета через подзорную трубу.
Если перейти от трубы с большим увеличением к более слабой, то **видимых деталей станет меньше, но сам предмет, конечно, никак от этого не изменится.**

Следующие преобразования являются расширяющими:
+ от класса A к классу B, если A наследуется от B (важным частным случаем является преобразование от любого ссылочного типа к Object);
+ от null-типа к любому объектному типу. 
 
 ![icon][nr]

[nr]:nr.png

 ![icon][string]

[string]:string.png

 ![icon][f]

[f]:f.png
 

# Methods "Overload" VS @Override

![icon][OO]

[OO]:OO.png

https://www.javatpoint.com/method-overloading-vs-method-overriding-in-java

# Пирамида тестирования

![icon][pyramid]

[pyramid]:pyramid.png

# Java Collection Framework (data structures)

Супер подробно тут:

https://github.com/Lapa-Lapa/java-interview/blob/master/jcf.md#java-collections-framework

Queue (очередь) предназначена для хранения элементов с предопределённым способом вставки и извлечения FIFO (first-in-first-out)

PriorityQueue — предоставляет возможность управлять порядком элементов в коллекции при помощи объекта Comparator, либо сохраняет элементы с использованием «natural ordering».

ArrayDeque — реализация интерфейса Deque, который расширяет интерфейс Queue методами, позволяющими реализовать конструкцию вида LIFO (last-in-first-out).

![icon][collections]

[collections]:collections.png

из лекции: https://www.youtube.com/watch?v=87pm79sPSvc&t=2155s

Java Arrays

String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};

Arrays are used to store multiple values in a single variable, instead of declaring separate variables for each value.

You access an array element by referring to the index number.

String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
cars[0] = "Opel";
System.out.println(cars[0]);
// Now outputs Opel instead of Volvo

Multidimensional Arrays

int[][] myNumbers = { {1, 2, 3, 4}, {5, 6, 7} };

int[][] myNumbers = { {1, 2, 3, 4}, {5, 6, 7} };
int x = myNumbers[1][2];
System.out.println(x); // Outputs 7

https://www.w3schools.com/java/java_arrays.asp

# LOCATORS

![icon][locators]

[locators]:locators.png

http://internetka.in.ua/selenium-webdriver-findelement-by/
http://internetka.in.ua/xpath-start-part1/
http://internetka.in.ua/xpath-start-part2/
http://internetka.in.ua/xpath-start-part3/
http://internetka.in.ua/xpath-start4/

# EXCEPTIONS

![icon][Exceptions]

[Exceptions]:Exceptions.png

https://github.com/Lapa-Lapa/java-interview/blob/master/core.md#%D0%A7%D1%82%D0%BE-%D1%82%D0%B0%D0%BA%D0%BE%D0%B5-checked-%D0%B8-unchecked-exception

# Heap и Stack

https://github.com/Lapa-Lapa/java-interview/blob/master/core.md#%D0%A7%D1%82%D0%BE-%D1%82%D0%B0%D0%BA%D0%BE%D0%B5-heap-%D0%B8-stack-%D0%BF%D0%B0%D0%BC%D1%8F%D1%82%D1%8C-%D0%B2-java-%D0%9A%D0%B0%D0%BA%D0%B0%D1%8F-%D1%80%D0%B0%D0%B7%D0%BD%D0%B8%D1%86%D0%B0-%D0%BC%D0%B5%D0%B6%D0%B4%D1%83-%D0%BD%D0%B8%D0%BC%D0%B8

Например такая команда сделает heap 512MB:

 -Xmx512m
 
 ![icon][Task_1]

[Task_1]:Task_1.png

-Xms: It is used for setting the initial and minimum heap size.

-Xmx: It is used for setting the maximum heap size.

Other JVM commands list could be see after "java -X" execution:

 ![icon][Task_2]

[Task_2]:Task_2.png

https://habr.com/ru/post/269707/

https://docs.oracle.com/cd/E19900-01/819-4742/abeik/index.html

https://alvinalexander.com/blog/post/java/java-xmx-xms-memory-heap-size-control/








# Tricky questions:

**How can you automate custom mouse or keyboard actions in WebDriver?**

package org.openqa.selenium.interactions;

public class Actions{

new Actions(WebDriverManager.getWebDriver()).moveToElement(getElement(), xOffset, yOffset).click().build().perform();

**How can you execute JavaScript code in WebDriver?**

String scriptResult = WebDriverUtils.callJavaScriptMethod("document.location");

**How to create WebDriver instance? RemoteWebDriver parameters?**

WebDriver webDriver = new ChromeDriver(ChromeOptions options);

public class ChromeDriver implements WebDriver interface so WebDriver instance will be creted

WebDriver driver = new RemoteWebDriver(URL remoteAddress, Capabilities capabilities);

**What is Selenium Grid?**

Selenium Grid is a testing tool which allows us to run our tests on different machines.

We are starting it from console/terminal by command:

java -jar selenium-server-standalone-2.53.0.jar -role hub -port 4444 -host 10.102.65.37

After opening http://10.102.65.37:4444/grid/console we will see grid with devices what were connected as nodes.

![icon][Grid]

[Grid]:Grid.png

When you execute your tests locally, the WebDriver client libraries talk to your Firefox Driver, IE Driver, or Chrome Driver directly. Now, when you try to execute your tests remotely, the WebDriver client libraries talk to the RemoteWebDriverserver and the server talks to either the Firefox Driver, IE Driver, or Chrome Driver, whichever the WebDriver client asks for.

https://www.toolsqa.com/selenium-webdriver/selenium-grid/

**What are typical steps to configure jobs in Jenkins?**
Source Code Management - выбрать Git например, указать URL репозитория, креды, ветку для кода.
Build Triggers - выбрать Build periodically

CRON *(min 0-59) *(hour 0-23) *(day 1-31) *(month 1-12) *(day of week 0-7[6=Saturday 0,7=Sunday])

*/5 * * * * - every 5 min

0 */2 * * * - every 2 hours

Post-build Actions - например залинковать вторую джобу, чтоб после билда тесты пошли например

**Можно ли создать объект абстрактного класса?** - нет

**Can interface extends class?** - yes. how many - one


**Какие типы методов есть в джаве:**

+ Стандартные, то есть написанные в стандартных библиотеках Java. Просто берешь нужный метод и используешь.

+ Пользовательские, то есть методы, которые Вы сами написали.


**Какие конструкторы есть:**

+ Явные (Явно прописывая конструктор, Вы получаете возможность регулировать, какие параметры и в каком количестве нужно задать для создания объекта определенного класса.)

+ Не явные (дефолтовые)

+ Закрытые (по другой классификации) (Иногда класс создаётся только для хранения каких-то статических полей и статических методов. Таким классам принято давать имена Utils, но это не обязательно. Такому классу не нужен конструктор, но если автор класса его не создал, то система сама создаст конструктор по умолчанию. Такой конструктор не имеет смысла, а также может послужить источником ошибок. Чтобы предохраниться от подобной проблемы вы сами явно должны создать пустрой конструктор и сделать его закрытым.)

+ Перегруженные (с this() еще называют Copy constructor - Язык программирования Java позволяет осуществлять вызов конструкторов класса из другого конструктора этого же класса. Для этого используется ключевое слово this, которое есть ссылкой на текущий класс.)

**Сколько раз бефор отрабатывает?** @Before (junit) annotation are executed before each test (No such annotation in TestNG = @BeforeMethod)
 ![icon][tng]

[tng]:tng.png

**Какая разница между регрессией и ретестингом?**
Повторное тестирование - фокусируется только на ранее неудачных тестовых случаях, но не обеспечивает полную проверку каждой функции, которую должно предоставить приложение.(Худший вариант для автоматизации)
Регресиионное тестирование - фокусируется на проверке, что свежие изменения в коде или приложении в целом не оказали негативного влияния на уже существующую функциональность/набор функций.(Идеально автотатизировать такие кейсы)