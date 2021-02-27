[Java Tutorials](README.md)

# JavaLanguages
+ [Какая основная идея языка?](#Какая-основная-идея-языка)
+ [За счет чего обеспечивается кроссплатформенность?](#За-счет-чего-обеспечивается-кроссплатформенность)
+ [Какие преимущества у java?](#Какие-преимущества-у-java)
+ [Какие недостатки у Java?](#Какие-недостатки-у-Java)
+ [Что такое JDK? Что в него входит?](#Что-такое-JDK-Что-в-него-входит)
+ [Что такое JRE? что в него входит?](#Что-такое-JRE-что-в-него-входит)
+ [Что такое JVM?](#Что-такое-JVM)
+ [Что такое byte code?](#Что-такое-byte-code)
+ [Что такое загрузчик классов (classloader)?](#Что-такое-загрузчик-классов-classloader)
+ [Что такое JIT?](#Что-такое-JIT)
+ [Что такое сборщик мусора? (Garbage collector)](#Что-такое-сборщик-мусора-Garbage-collector)
+ [Что такое Heap и Stack память в Java? Чем они отличаются?](#Что-такое-Heap-и-Stack-память-в-Java-Чем-они-отличаются)
+ [Виды ссылок в Java](#Виды-ссылок-в-Java)

+ [ССЫЛКИ НА ДОПОЛНИТЕЛЬНУЮ ИНФУ](#ССЫЛКИ-НА-ДОПОЛНИТЕЛЬНУЮ-ИНФУ)
[к оглавлению](#javaLanguages)


## Какая основная идея языка?
«Написано однажды - работает везде».
Идея основывается в написании одного кода, который будет работать на любой платформе.
+ [к оглавлению](#javaLanguages)

## За счет чего обеспечивается кроссплатформенность?
Кроссплатформенность была достигнута за счёт создания виртуальной машины Java. `Java Virtual Machine` или `JVM` - это программа, являющаяся прослойкой между операционной системой и Java программой. В среде виртуальной машины выполняются коды Java программ. Сама `JVM` реализована для разных ОС.
+ [к оглавлению](#javaLanguages)

## Какие преимущества у java?
__1) Объектно-ориентированное программирование__   
+ структура данных становится объектом, которым можно управлять для создания отношений между различными объектами.

__2) Язык высокого уровня с простым синтаксисом и плавной кривой обучения__ 
+ синтаксис Java основан на C++, поэтому Java похожа на C. Тем не менее, синтаксис Java проще, что позволяет новичкам быстрее учиться и эффективнее использовать код для достижения конкретных результатов.

__3) Стандарт для корпоративных вычислительных систем__
+ корпоративные приложения — главное преимущество Java с 90-х годов, когда организации начали искать надежные инструменты программирования не на C.

__4) Безопасность__ 
+ благодарю отсутсвию указателей и `Security Manager` (политика безопасности, в которой можно указать правила доступа, позволяет запускать приложения Java в "песочнице").

__5) Независимость от платформы__ 
+ Можно создать Java-приложение на Windows, скомпилировать его в байт-код и запустить его на любой другой платформе, поддерживающей виртуальную машину Java (`JVM`). Таким образом, `JVM` служит уровнем абстракции между кодом и оборудованием.

__6) Язык для распределенного программирования и комфортной удаленной совместной работы__
+ Специфическая для Java методология распределенных вычислений называется `Remote Method Invocation (RMI)`. `RMI` позволяет использовать все преимущества Java: безопасность, независимость от платформы и объектно-ориентированное программирование для распределенных вычислений. Кроме того, Java также поддерживает программирование сокетов и методологию распределения CORBA для обмена объектами между программами, написанными на разных языках.

__7) Автоматическое управление памятью__
+ Разработчикам Java не нужно вручную писать код для управления памятью благодаря 
автоматическому управлению памятью (`AMM`).

__8) Многопоточность__
+ Поток — наименьшая единица обработки в программировании. Чтобы максимально эффективно использовать время процессора, Java позволяет запускать потоки одновременно, что называется многопоточностью.

__9) Стабильность и сообщество__
+ Сообщество разработчиков Java не имеет себе равных. Около 45% респондентов опроса StackOverflow 2018 используют Java.
+ [к оглавлению](#javaLanguages)

## Какие недостатки у Java?
__1) Платное коммерческое использование (с 2019)__

__2) Низкая производительность__
+ из-за компиляции и абстракции с помощью виртуальной машины, а также приложение очистки памяти.

__3) Не развитые инструменты по созданию GUI приложений на чистой java.__

__4) Многословный код__
+ Java — это более легкая версия неприступного C ++, которая вынуждает программистов прописывать свои действия словами из английского языка. Это делает язык более понятным для неспециалистов, но менее компактным.
+ [к оглавлению](#javaLanguages)

## Что такое JDK? Что в него входит?
__JDK (Java Development Kit) - включает `JRE` и набор инструментов разработчика приложений на языке Java:__
- компилятор Java (javac)
- стандартные библиотеки классов java
- примеры
- документацию
- различные утилиты
+ [к оглавлению](#javaLanguages)

## Что такое JRE? что в него входит?
__JRE (java Runtime Environment)__ - минимально-необходимая реализация виртуальной машины для исполнения Java-приложений. Состоит из `JVM`, `ClassLoader` и стандартного набора библиотек и классов Java
+ [к оглавлению](#javaLanguages)

## Что такое JVM?
__JVM (Java Virtual Machine)__ - виртуальная машина Java исполняет байт-код Java, предварительно созданный из кода `JIT компилятором`, с помощью встроенного интерпретатора байткода.
`HotSpot` представляет собой реализацию концепции `JVM`.
+ [к оглавлению](#javaLanguages)

## Что такое byte code?	
Байт-код Java — набор инструкций, скомпилированный компилятором, исполняемый `JVM`.
+ [к оглавлению](#javaLanguages)

## Что такое загрузчик классов (classloader)?
Используется для передачи в `JVM` скомпилированного байт-кода, хранится в файлах с расширением `.class`

__При запуске `JVM`, используются три загрузчика классов:__

__1) Bootstrap ClassLoader__ - базовый загрузчик
- загружает платформенные классы JDK из архива `rt.jar`

__2) AppClassLoader__ - системный загрузчик
- загружает классы приложения, определенные в `CLASSPATH` 

__3) Extension ClassLoader__ - загрузчик расширений 
- загружает классы расширений, которые по умолчанию находятся в каталоге `jre/lib/ext`.

__ClassLoader выполняет три основных действия в строгом порядке:__

__1) Загрузка:__ находит и импортирует двоичные данные для типа.

__2) Связывание:__ выполняет проверку, подготовку и (необязательно) разрешение.
+ Проверка: обеспечивает правильность импортируемого типа.
+ Подготовка: выделяет память для переменных класса и инициализация памяти значениями по умолчанию.
+ Разрешение: преобразует символические ссылки из типа в прямые ссылки.

__3) Инициализация:__ вызывает код Java, который инициализирует переменные класса их правильными начальными значениями.

Каждый загрузчик хранит указатель на родительский, чтобы суметь передать загрузку если сам будет не в состоянии этого сделать
+ [к оглавлению](#javaLanguages)

## Что такое JIT?
JIT (Just-in-time compilation) - компиляция на лету или динамическая компиляция - технология увеличения производительности программных систем, использующих байт-код, путем компиляции байт-кода в машинный код во время работы программы.
+ [к оглавлению](#javaLanguages)

## Что такое сборщик мусора? (Garbage collector)
Сборщик мусора выполняет две задачи:
+ поиск мусора;
+ очистка мусора.

Для обнаружения мусора есть два подхода:

__1) Учет ссылок (Reference counting);__
+ Учет ссылок - если обьект не имеет ссылок, он считается мусором.
Проблема - не возможность выявить циклические ссылки, когда два обьекта не имеют внешних ссылок, но ссылаются друг на друга -> утечка памяти

__2) Трассировка (Tracing). (используется в HotSpot6)__
+ Трассировка - до обьекта можно добраться из Корневых точек (GC root). 
До чего добраться нельзя - мусор.
Всё, что доступно из «живого» объекта, также является «живым».

__Типы корневых точек (GC Roots) java приложения:__
+ объекты в статических полях классов
+ объекты, доступные из стека потоков
+ объекты из JNI(java native interface) ссылок в native методах

__Процессы сборки мусора разделяются на несколько видов:__

__1) minor GC (малая)__ - частый и быстрый, работает только с областью памяти "`young generation`";
+ приложение приостанавливается на начало сборки мусора (такие остановки называются stop-the-world);
+ «живые» объекты из Eden перемещаются в область памяти «To»;
+ «живые» объекты из «From» перемещаются в «To» или в «old generation», если они достаточно «старые»;
+ Eden и «From» очищаются от мусора;
+ «To» и «From» меняются местами;
+ приложение возобновляет работу.

__2) major GC (старшая)__ - редкий и более длительный, затрагивает объекты старшего поколения.
В принцип работы «major GC» добавляется процедура «уплотнения», позволяющая более эффективно использовать память. В процедуре живые объекты перемещаются в начало. Таким образом, мусор остается в конце памяти.

__3) full GC (полная)__ -  полный сборщик мусора сначала запускает Minor, а затем Major (хотя порядок может быть изменен, если старое поколение заполнено, и в этом случае он освобождается первым, чтобы позволить ему получать объекты от молодого поколения).

Про 4 типа сборщиков мусора читай сдесь: habr.com/ru/post/269621
+ [к оглавлению](#javaLanguages)

## Что такое Heap и Stack память в Java? Чем они отличаются?
__Память процесса делится на `Stack(стек)` и `Heap(куча)` :__
- `Stack` содержит `staсk frame'ы`, они делятся на три части: параметры метода, указатель на предыдущий фрейм и локальные переменные.
- Структура `Heap` зависит от выбранного сборщика мусора. Читай про GC!

`MetaSpace` - специальное пространство кучи, отделенное от кучи основной памяти. `JVM` хранит здесь весь статический контент. Это включает в себя все статические методы, примитивные переменные и ссылки на статические объекты. Кроме того, он содержит данные о байт-коде, именах и `JIT-информации` . До Java 7 `String Pool` также был частью этой памяти. 

С помощью опций `Xms` и `Xmx` можно настроить начальный и максимально допустимый размер кучи соответственно. Существуют опции для настройки величины стека.
- `Heap` - используется всем приложением, `Stack` - одним потоком исполняемой программы.
- Новый обьект создается в `heap`, в `stack` размещается ссылка на него. В стеке размещаются локальные переменные примитивных типов. 
- Обьекты в куче доступны из любого места программы, стековая память не доступна для других потоков.
- Если память стека закончилась `JRE` вызовет исключение `StackOverflowError`, если куча заполнена `OutOfMemoryError`
- Размер памяти стека, меньше памяти кучи. Стековая память быстрее памяти кучи.
- В куче есть ссылки между объектами и их классами. На этом основана рефлексия.

Обе области хранятся в RAM.
+ [к оглавлению](#javaLanguages)

## Виды ссылок в Java

__1) StrongReference__ — это самые обычные ссылки которые мы создаем каждый день, любая переменная ссылочного типа.
        StringBuilder builder = new StringBuilder(); - builder это и есть strong-ссылка на объект StringBuilder.
        
__2) SoftReference__ —  GC гарантировано удалит с кучи все объекты, доступные только по soft-ссылке, перед тем как бросит `OutOfMemoryError`. `SoftReference` это наш механизм кэширования объектов в памяти, но в критической ситуации, когда закончится доступная память, GC удалит не использующиеся объекты из памяти и тем самым попробует спасти JVM от завершения работы.
        StringBuilder builder = new StringBuilder();
        SoftReference<StringBuilder> softBuilder = new SoftReference(builder);

softBuilder.get() — вернет strong-ссылку на объект StringBuilder в случае если GC не удалил этот объект из памяти. В другом случае вернется null.
softBuilder.clear() — удалит ссылку на объект StringBuilder
То же самое работает для WeakReference.

__3) WeakReference__ — если GC видит, что объект доступен только через цепочку weak-ссылок (исчезли strong-ссылки), то он удалит его из памяти

__4) PhantomReference__ — если GC видит что объект доступен только через цепочку phantom-ссылок, то он его удалит из памяти. После нескольких запусков GC.
Особенностей у этого типа ссылок две.
+ Первая это то, что метод get() всегда возвращает null. Именно из-за этого `PhantomReference` имеет смысл использовать только вместе с `ReferenceQueue`.
+ Вторая особенность – в отличие от `SoftReference` и `WeakReference`, GC добавит phantom-ссылку в `ReferenceQueue` после того как выполниться метод `finalize()`.

So in brief: Soft references try to keep the reference. Weak references don’t try to keep the reference. Phantom references don’t free the reference until cleared

__ReferenceQueue.__ Он позволяет отслеживать момент, когда GC определит что объект более не нужен и его можно удалить. Именно сюда попадает Reference объект после того как объект на который он ссылается удален из памяти. При создании `Reference` мы можем передать в конструктор `ReferenceQueue`, в который будут помещаться ссылки после удаления
+ [к оглавлению](#javaLanguages)


## ССЫЛКИ НА ДОПОЛНИТЕЛЬНУЮ ИНФУ

#### [Название-->]( Ссылка )
#### [Название-->]( Ссылка )
#### [Название-->]( Ссылка )
#### [Название-->]( Ссылка )
#### [Название-->]( Ссылка )
#### [Название-->]( Ссылка )
#### [Название-->]( Ссылка )

+ [к оглавлению](#javaLanguages)