[Java Tutorials](README.md)

# ProceduralJava
1) [Сколько ключевых слов зарезервировано языком, что это за слова, какие из них не используются?](#Сколько-ключевых-слов-зарезервировано-языком-что-это-за-слова-какие-из-них-не-используются)
2) [Из каких символов может состоять имя переменной (корректный идентификатор)?](#Из-каких-символов-может-состоять-имя-переменной-корректный-идентификатор)
3) [Какие примитивные типы данных есть в Java?](#Какие-примитивные-типы-данных-есть-в-Java)
4) [Что такое char?](#Что-такое-char)
5) [Сколько памяти занимает boolean?](#Сколько-памяти-занимает-boolean)
6) [Что такое классы-обертки (Wrapper Class)?](#Что-такое-классы-обертки-Wrapper-Class)
7) [Что такое автоупаковка и автораспаковка?](#Что-такое-автоупаковка-и-автораспаковка)
8) [Что такое явное и неявное приведение типов? В каких случаях в java нужно использовать явное приведение?](#Что-такое-явное-и-неявное-приведение-типов-В-каких-случаях-в-java-нужно-использовать-явное-приведение) 
9) [Что такое пул интов?](#Что-такое-пул-интов)
10) [Какие нюансы у строк в Java?](#Какие-нюансы-у-строк-в-Java)
11) [Что такое пул строк?](#Что-такое-пул-строк)
12) [Почему не рекомендуется изменять строки в цикле? Что рекомендуется использовать?](#Почему-не-рекомендуется-изменять-строки-в-цикле-Что-рекомендуется-использовать)
13) [Почему строки не рекомендуется использовать для хранения паролей?](#Почему-строки-не-рекомендуется-использовать-для-хранения-паролей)
14) [Почему `String` неизменяемый и финализированный класс?](#Почему-string-неизменяемый-и-финализированный-класс)
15) [Почему строка является популярным ключом в `HashMap` в Java?](#Почему-строка-является-популярным-ключом-в-hashmap-в-java)
16) [Что делает метод `intern()` в классе `String`?.](#Что-делает-метод-intern-в-классе-string)
17) [Можно ли использовать строки в конструкции `switch`?](#Можно-ли-использовать-строки-в-конструкции-switch)
18) [Какая основная разница между `String`, `StringBuffer`, `StringBuilder`?](#Какая-основная-разница-между-string-stringbuffer-stringbuilder)
19) [Методы класса `String`?](#Методы-класса-String)
20) [Методы класса `Character`?](#Методы-класса-Character)
21) [Существуют ли в java многомерные массивы?](#Существуют-ли-в-java-многомерные-массивы)
22) [Какими значениями инициируются переменные по умолчанию?](#Какими-значениями-инициируются-переменные-по-умолчанию)
23) [Что такое сигнатура метода?](#Что-такое-сигнатура-метода)
24) [Расскажите про метод main](#Расскажите-про-метод-main)
25) [Каким образом переменные передаются в методы, по значению или по ссылке?](#Каким-образом-переменные-передаются-в-методы-по-значению-или-по-ссылке)
26) [Для чего используется оператор `assert`?](#Для-чего-используется-оператор-assert)
27) [Какие логические операции и операторы вы знаете?](#Какие-логические-операции-и-операторы-вы-знаете)
28) [Что такое тернарный оператор выбора?](#Что-такое-тернарный-оператор-выбора)
29) [Какие побитовые операции вы знаете?](#Какие-побитовые-операции-вы-знаете)
30) [Какие унарные и бинарные арифметические операции вы знаете?](#Какие-унарные-и-бинарные-арифметические-операции-вы-знаете)
31) [Какова роль и правила написания оператора выбора (switch)?](#Какова-роль-и-правила-написания-оператора-выбора-switch)
32) [Какие циклы вы знаете, в чем их отличия?](#Какие-циклы-вы-знаете-в-чем-их-отличия)
33) [Какие операторы используются для перехода к следующей итерации и немедленной остановки цикла?](#Какие-операторы-используются-для-перехода-к-следующей-итерации-и-немедленной-остановки-цикла)
+ [ССЫЛКИ НА ДОПОЛНИТЕЛЬНУЮ ИНФУ](#ССЫЛКИ-НА-ДОПОЛНИТЕЛЬНУЮ-ИНФУ)
+ [к оглавлению](#ProceduralJava)


## Сколько ключевых слов зарезервировано языком, что это за слова, какие из них не используются?
50, два из них не используются: const, goto;

Для запоминания это:
+ Примитивы (byte, short, int, long, char, float, double, boolean)
+ Циклы и ветвления (if, else, switch, case, default, while, do, break, continue, for)
+ Исключения (try, catch, finally, throw, throws)
+ Области видимости (private, protected, public)
+ Объявление \ Импорт (import, package, class, interface, extends, implements, static, final, void, abstract, native)
+ Создание \ Возврат \ Вызов (new, return, this, super)
+ Многопоточность (synchronized, volatile)
+ instanceof, enum, assert, transient, strictfp, const, goto

http://docs.oracle.com/javase/tutorial/java/nutsandbolts/_keywords.html

+ [Вопрос#1  К оглавлению](#ProceduralJava)

## Из каких символов может состоять имя переменной (корректный идентификатор)?
Имя или идентификатор переменной — это последовательность из строчных и заглавных латинских букв, цифр, а также символов «$» и «_». Имя переменной может начинаться с любого из перечисленных символов, кроме цифры.

Технически возможно начать имя переменной также с «$» или «_», однако это запрещено соглашением по оформлению кода в Java (Java Code Conventions). Кроме того, символ доллара «$», по соглашению, никогда не используется вообще. В соответствии с соглашением имя переменной должно начинаться именно с маленькой буквы (с заглавной буквы начинаются имена классов). Пробелы при именовании переменных не допускаются.
+ [Вопрос#2  К оглавлению](#ProceduralJava)

## Какие примитивные типы данных есть в Java?
__Вещественные, целочисленные, логические, строковые__

Примитивные:
+ byte (целые числа, 1 байт, [-128, 127])
+ short (целые числа, 2 байта, [-32768, 32767])
+ int (целые числа, 4 байта, [-2147483648, 2147483647])
+ long (целые числа, 8 байт, [-9223372036854775808,9223372036854775807])
+ float (вещественные числа, 4 байта)
+ double (вещественные числа, 8 байт)
+ char (символ Unicode, 2 байта, [0, 65536])
+ boolean (значение истина/ложь, используется int, зависит от JVM)

Ссылочные. В ссылочные типы входят все классы, интерфейсы, массивы.

http://stackoverflow.com/questions/383551/what-is-the-size-of-a-boolean-variable-in-java
boolean type: http://docs.oracle.com/javase/specs/jvms/se8/html/jvms-2.html#jvms-2.3.4
boolean — боремся за Java память… https://habrahabr.ru/post/76481/

+ [Вопрос#3  К оглавлению](#ProceduralJava)

## Что такое char?
16-разрядное беззнаковое целое, представляющее собой символ UTF-16 (буквы и цифры)
+ [Вопрос#4  К оглавлению](#ProceduralJava)

## Сколько памяти занимает boolean?
Зависит от реализации JVM
В стандартной реализации Sun JVM и Oracle HotSpot JVM тип boolean занимает 4 байта (32 бита), как и тип int. Однако, в определенных версия JVM имеются реализации, где в массиве boolean каждое значение занимает по 1-му биту.
Также есть библиотеки для уменьшения размера boolean: BitSet и OpenBitSet (от Apache).
Тип boolean прекрасно определяется множеством своих допустимых значений. Математически оно ограничивает минимальный размер значения одним битом.

Но использовать именно один бит (и ни битом более) эффективно далеко не всегда, поскольку на популярных архитектурах нельзя адресовать отдельные биты. А потому значения отдельных boolean'ов нельзя быстро сохранить в отдельные биты оперативной памяти — необходимо использовать комбинацию побитовых операций, что почти наверняка будет медленнее, чем запись целого отдельного регистра в оперативную память (размер которого может быть различным на разных платформах!).

Но при этом, к примеру, я вполне себе представляю, как на x86 компилятор может использовать в нативном коде в качестве какого-нибудь конкретного boolean-значения один бит регистра флагов, при условии, что это значение никогда не попадает в оперативную память (отдельно от других). Поэтому любые ограничения на размер более одного бита тоже могут потенциально мешать.

И эта свобода представления позволяет авторам виртуальных машин Java использовать любые реализации, которые они считают наиболее эффективными в каждом конкретном контексте. Как видно из примеров выше, любые ограничения будут только мешать.
+ [Вопрос#5  К оглавлению](#ProceduralJava)

## Что такое классы-обертки (Wrapper Class)?
Обертка — это специальный класс, который хранит внутри себя значение примитива.
Нужны для реализации дженериков.
Популярные методы:
+ Double.parseDouble(a);//пожалуй, самый популярный метод перевод из строки в целочисленный или дробный тип
+ System.out.println(Integer.MAX_VALUE);//константа максимального значения
+ System.out.println(Integer.bitCount(78));// в двоичном виде
+ System.out.println(Float.valueOf("80"));//возвращает целочисленный объект, содержащий значение указанного типа
Хотелось бы еще рассмотреть создание Boolean переменной:
```java
public class BooleanExample {
    public static void main(String[] args){
        Boolean b1 = new Boolean(false);//false
        Boolean b2 = new Boolean("false");//false
        Boolean b3 = new Boolean(true);//true
        Boolean b4 = new Boolean("true");//true
        Boolean b5 = new Boolean("hi there");//false
    }
}
```
+ [Вопрос#6  К оглавлению](#ProceduralJava)

## Что такое автоупаковка и автораспаковка?
__Автоупаковка__ - присвоение классу обертки значения примитивного типа;
__Автораспаковка__ - присвоение переменной примитивного типа значение класса обертки.

Для присваивания ссылок-примитивов объектам их классов-оберток (и наоборот) не требуется ничего делать, все происходит автоматически.

__Автоупаковка__ - это механизм неявной инициализации объектов классов-оберток (`Byte`, `Short`, `Integer`, `Long`, `Float`, `Double`, `Character`, `Boolean`) значениями соответствующих им исходных примитивных типов (`byte`, `short`, `int`...), без явного использования конструктора класса. 

+ Автоупаковка происходит при прямом присваивании примитива классу-обертке (с помощью оператора `=`), либо при передаче примитива в параметры метода (типа класса-обертки). 

+ Автоупаковке в классы-обертки могут быть подвергнуты как переменные примитивных типов, так и константы времени компиляции (литералы и `final`-примитивы). При этом литералы должны быть синтаксически корректными для инициализации переменной исходного примитивного типа.

+ Автоупаковка переменных примитивных типов требует точного соответствия типа исходного примитива типу класса-обертки. Например, попытка упаковать переменную типа `byte` в `Short`, без предварительного явного приведения `byte` в `short` вызовет ошибку компиляции.

+ Автоупаковка констант примитивных типов допускает более широкие границы соответствия. В этом случае компилятор способен предварительно осуществлять неявное расширение/сужение типа примитивов:
    1) неявное расширение/сужение исходного типа примитива до типа примитива соответствующего классу-обертке (для преобразования `int` в `Byte`, сначала компилятор самостоятельно неявно сужает `int` к `byte`)
    2) автоупаковку примитива в соответствующий класс-обертку. Однако, в этом случае существуют два дополнительных ограничения:
        a) присвоение примитива обертке может производится только оператором `=` (нельзя передать такой примитив в параметры метода без явного приведения типов)
        b) тип левого операнда не должен быть старше чем `Character`, тип правого не дожен старше, чем `int`: допустимо расширение/сужение `byte` в/из `short`, `byte` в/из `char`, `short` в/из `char` и только сужение `byte` из `int`, `short` из `int`, `char` из `int`. Все остальные варианты требуют явного приведения типов).

Дополнительной особенностью целочисленных классов-оберток, созданных автоупаковкой констант в диапазоне `-128 ... +127` я вляется то, что они кэшируются JVM. Поэтому такие обертки с одинаковыми значениями будут являться ссылками на один объект.
+ [Вопрос#7  К оглавлению](#ProceduralJava)

## Что такое явное и неявное приведение типов? В каких случаях в java нужно использовать явное приведение?
__Неявное приведение__ – автоматическое расширение типа переменной от меньшего к большему.
__Явное приведение__ -  явное сужение от большего к меньшему. Необходимо явно указать сужаемый тип.
В случае с объектами мы можем делать неявное(автоматическое) приведение от наследника к родителю, но не наоборот, иначе получим ClassCastException.

Преобразование может быть неявным и явным (приведение типов). Неявное преобразование может выполняться если:
типы совместимы (например – оба целочисленные)
размер “принимающего” типа больше чем у того, который преобразуется (так называемое “преобразование с расширением”)
```java
int a = 123454;
double b =  a; //неявное преобразование - преобразование с расширением
int a = 123454;
double b =  a; //неявное преобразование - преобразование с расширением

Явное преобразование имеет вид переменная_нового_типа = (новый_тип) имя переменной;
int a;
byte b = (byte) a; //b будет остатком от деления a на диапазон byte, может быть потеря данных
int a;
byte b = (byte) a; //b будет остатком от деления a на диапазон byte, может быть потеря данных
```
Примеры:
```java
public static void typeConverterExample() {
        long a = 100L;
        double b = 300.0;
        Object ab = a + b;
        System.out.println(ab.getClass().getName() + " value: " + ab); //java.lang.Double value: 400.0

        double c = 1000.05;
        long d = 1000;
        Object cd = c+d;
        System.out.println(cd.getClass().getName() +" value: " + cd);//java.lang.Double value: 2000.05
    }

    public static void typeNarrowing() {
        int a0 = 64;
        int a = 257;
        int a2 = 126;
        int a3 = 129;
        byte b0 = (byte) a0;
        byte b = (byte) a;
        byte b2 = (byte) a2;
        byte b3 = (byte) a3;
        System.out.println(b0+ " " + b + " " + b2 + " " + b3); //64 1 126 -127

        double c = 56.9876;
        int d = (int) c;
        System.out.println(d); //56

        long e = 1000L;
        float f = (float) e;
        System.out.println(f); //1000.0
    }

public static void typeConverterExample() {
        long a = 100L;
        double b = 300.0;
        Object ab = a + b;
        System.out.println(ab.getClass().getName() + " value: " + ab); //java.lang.Double value: 400.0
 
        double c = 1000.05;
        long d = 1000;
        Object cd = c+d;
        System.out.println(cd.getClass().getName() +" value: " + cd);//java.lang.Double value: 2000.05
    }
 
    public static void typeNarrowing() {
        int a0 = 64;
        int a = 257;
        int a2 = 126;
        int a3 = 129;
        byte b0 = (byte) a0;
        byte b = (byte) a;
        byte b2 = (byte) a2;
        byte b3 = (byte) a3;
        System.out.println(b0+ " " + b + " " + b2 + " " + b3); //64 1 126 -127
 
        double c = 56.9876;
        int d = (int) c;
        System.out.println(d); //56
 
        long e = 1000L;
        float f = (float) e;
        System.out.println(f); //1000.0
    }
```
При повышении типа byte>short; short>int; int>long; float>double; char>int информация не потеряется. При сужении возможна потеря информации (см. пример выше byte = (byte) int).

При различных операциях может происходить повышение типов в порядке “усиления” к более информативному типу. Например складывая int и double получим тип double. Но есть и особенность, например сложив double (8 байт) и long (8 байт) Java оставит знаки после запятой (double), а не более “длинный” тип. Аналогичный пример с вещественной частью:
```java
  long a = 100L;
        double b = a;
        Object ab = a + b;
        System.out.println(ab.getClass().getName() + " value: " + ab); //java.lang.Double value: 200.0

        float c = 100;
        long d = 1000;
        Object cd = c - d;
        System.out.println(cd.getClass().getName() +" value: " + cd);//java.lang.Float value: -900.0

  long a = 100L;
        double b = a;
        Object ab = a + b;
        System.out.println(ab.getClass().getName() + " value: " + ab); //java.lang.Double value: 200.0
 
        float c = 100;
        long d = 1000;
        Object cd = c - d;
        System.out.println(cd.getClass().getName() +" value: " + cd);//java.lang.Float value: -900.0
```
Кратко можно записать такие правила:
+ byte, short, char в выражениях всегда повышаются до int
+ если в выражении участвует тип long – то именно к этому типу будет приведён результат
+ если в выражении участвует float – то результат приводится к float
+ если один из операндов имеет тип double – то к этому типу будет приведён весь результат
+ При выборе между длиной и возможностью сохранить дробную часть – будет выбрана дробная часть

+ [Вопрос#8  К оглавлению](#ProceduralJava)

## Что такое пул интов?
В Java есть пул(pool) целых чисел в промежутке [-128;127], так как это самый часто вречающийся диапазон. Т.е. если мы создаем Integer в этом промежутке, то вместо того, чтобы каждый раз создавать новый объект, JVM берет их из пула. 
Изменить размер кэша в HotSpot вы можете, указав ключ -XX:AutoBoxCacheMax=<размер>.
+ [Вопрос#9  К оглавлению](#ProceduralJava)

## Какие нюансы у строк в Java?
Класс `String` в Java -  неизменяемый из-за модификатора `final` и отсутствия сеттера. Это нужно для реализации пула стрингов. При редактировании будет создаваться новая строка. При копировании новая строка не создается, а создается ссылка на существующую строку.
+ Это неизменяемый (immutable) и финализированный тип данных;
+ Все объекты класса `String` JVM хранит в пуле строк;
+ Объект класса `String` можно получить, используя двойные кавычки;
+ Можно использовать оператор `+` для конкатенации строк;
+ Начиная с Java 7 строки можно использовать в конструкции `switch`.

+ [Вопрос#10  К оглавлению](#ProceduralJava)

## Что такое пул строк?
__Область памяти где хранятся обьекты строк.__ 
При создании в пуле идет поиск строки:
+ если НЕ находит -  создается строка, возращается ссылка
+ если находит - возращает ссылку найденной строки.

При этом использование оператора `new` заставляет класс `String` создать новый объект, даже если такая строка уже есть в пуле. После этого можем использовать метод `intern()`, чтобы поместить этот объект в пул строк.

Пул строк и `Integer` хранится в heap, но ссылки на объекты хранятся в `stack`.
+ [Вопрос#11  К оглавлению](#ProceduralJava)

## Почему не рекомендуется изменять строки в цикле? Что рекомендуется использовать?
Т.к. строка неизменяемый класс, потребление ресурсов при редактировании, т.к. каждую итерацию при редактировании будет создаваться новый обьект строки. 
Рекомендуется использовать `StringBuilder`
+ [Вопрос#12  К оглавлению](#ProceduralJava)

## Почему строки не рекомендуется использовать для хранения паролей?
1) __Строки — неизменны__
Так как строки в Java являются неизменными, то ваш пароль в виде обычного текста будет доступен в памяти, пока сборщик мусора не очистит её. И поскольку `String `используются в `String pool` для повторного использования, существует довольно высокая вероятность того, что пароль останется в памяти надолго, что совсем не безопасно. 

2) __Рекомендации авторов__
Java сама по себе рекомендует использовать метод `getPassword ()` из класса `JPasswordField`, который возвращает `char []`.
В случае использования массива символов для хранения пароля имеется возможность очистить его сразу по окончанию работы с паролем, позволяя избежать риска безопасности, свойственного строке.

3) __Случайная печать в логах__
С типом String всегда существует опасность того, что текст, хранящийся в строке будет напечатан в файле логов или в консоли. В то же время в случае использования `Array`, вы не будете печатать содержимое массива, а только его расположение в памяти.

+ [Вопрос#13  К оглавлению](#ProceduralJava)

## Почему `String` неизменяемый и финализированный класс?
Есть несколько преимуществ в неизменности строк:

1) __Для возможности реализации строкового пула (`String pool`)__

Виртуальная машина имеет возможность сохранить много места в памяти (`heap space`) т.к. разные строковые переменные указывают на одну переменную в пуле. При изменяемости строк было бы невозможно реализовать интернирование, поскольку если какая-либо переменная изменит значение, это отразится также и на остальных переменных, ссылающихся на эту строку.

2) __Безопасность__

Изменяемость строк несло бы в себе потенциальную угрозу безопасности приложения. Поскольку в Java строки используются для передачи параметров для авторизации, открытия файлов и т.д. — неизменяемость позволяет избежать проблем с доступом.

3) __Для многопоточности. Неизменяемые строки потокобезопасны__

Так как строка неизменяемая то, она безопасна для много поточности и один экземпляр строки может быть совместно использован различными потоками. Это позволяет избежать синхронизации для потокобезопасности. Таким образом, строки в Java полностью потокобезопасны.

4) __Ключ для HashMap__

Поскольку строка неизменная, её hashcode кэшируется в момент создания и нет никакой необходимости рассчитывать его снова. Это делает строку отличным кандидатом для ключа в `Map` и его обработка будет быстрее, чем других ключей `HashMap`. Поэтому строка наиболее часто используется в качестве ключа `HashMap`.

5) Строки используются `_classloader_` и неизменность обеспечивает правильность загрузки класса.

+ [Вопрос#14  К оглавлению](#ProceduralJava)

## Почему строка является популярным ключом в `HashMap` в Java?
Поскольку строки неизменяемы, их хэш код вычисляется и кэшируется в момент создания, не требуя повторного пересчета при дальнейшем использовании. Поэтому в качестве ключа `HashMap` они будут обрабатываться быстрее.
+ [Вопрос#15  К оглавлению](#ProceduralJava)

## Что делает метод `intern()` в классе `String`?
Метод `intern()` используется для сохранения строки в пуле строк или получения ссылки, если такая строка уже находится в пуле.
+ [Вопрос#16  К оглавлению](#ProceduralJava)

## Можно ли использовать строки в конструкции `switch`?
Да, начиная с Java 7 в операторе `switch` можно использовать строки, ранние версии Java не поддерживают этого. При этом:

+ участвующие строки чувствительны к регистру;
+ используется метод `equals()` для сравнения полученного значения со значениями `case`, поэтому во избежание `NullPointerException` стоит предусмотреть проверку на `null`.
+ согласно документации, Java 7 для строк в `switch`, компилятор Java формирует более эффективный байткод для строк в конструкции `switch`, чем для сцепленных условий `if`-`else`.
+ должно присутствовать ключевое слово `default`

+ [Вопрос#17  К оглавлению](#ProceduralJava)

## Какая основная разница между `String`, `StringBuffer`, `StringBuilder`?
Класс `String`(НЕизменяемый, потобезопасный) является неизменяемым (_immutable_) - модифицировать объект такого класса нельзя, можно лишь заменить его созданием нового экземпляра.

Класс `StringBuffer` (изменяемый, потокобезопасный) - использовать `StringBuffer` следует тогда, когда необходимо часто модифицировать содержимое. 

Класс `StringBuilder` (изменяемый, НЕпотокобезопасный) - был добавлен в Java 5 и он во всем идентичен классу `StringBuffer` за исключением того, что он не синхронизирован и поэтому его методы выполняются значительно быстрей.

+ [Вопрос#18  К оглавлению](#ProceduralJava)

## Методы класса `String`?
+ str.length(); - возвращает длину строки
+ str.replaceAll(Character.toString(ch), ""); - для замены всех вхождений в строку другой строкой
+ toUpperCase / toLowerCase - изменение регистра строки
+ subSequence внутри вызывает метод substring и выделяет подстроку из строки
+ equals(String str) метод сравнения строк
+ compareTo(String anotherString) - сравнивает объект String с полученным аргументом String лексикографически. Если текущая строка предшествует полученной строке, метод возвращает отрицательное значение типа integer, и если строка следует за полученным аргументом, то возвращает положительное значение integer. Если метод возвращает 0, значит строка имеет то же значение, в таком случае метод equals(String str) так же вернет true
+ char c = str.charAt(1); - метод для получения символа, находящегося в указанной позиции
+ char[] chArr = str.toCharArray(); - для преобразования строки в массив символов
+ byte[] byteArr = str.getBytes(); - для преобразования строки в массив байтов
+ String[] words = line.split(" "); - для разделения строки на массив строк, используя в качестве разделителя регулярное выражение.
+ String c = b.intern(); - если пул строк уже содержит строку, эквивалентную к нашему объекту, что подтверждается методом equals(Object), тогда возвращается ссылка на строку из пула. В противном случае объект строки добавляется в пул и ссылка на этот объект возвращается

+ [Вопрос#19  К оглавлению](#ProceduralJava)

## Методы класса `Character`?
+ boolean isLetter (char ch) : этот метод используется для определения, является ли указанное значение char (ch) буквой или нет
+ boolean isDigit (char ch) : этот метод используется для определения, является ли указанное значение char (ch) цифрой или нет
+ boolean isWhitespace (char ch ) : определяет, является ли указанное значение char (ch) пробелом
+ boolean isUpperCase (char ch) : определяет, является ли указанное значение char (ch) заглавными или нет.
+ boolean isLowerCase (char ch) : определяет, является ли указанное значение char (ch) строчными или нет.
+ toString (char ch) : возвращает объект класса String, представляющий указанное символьное значение (ch), то есть односимвольную строку. Здесь мы не можем передать значение ASCII.
+ char charValue () : этот метод возвращает значение этого объекта Character.

+ [Вопрос#20  К оглавлению](#ProceduralJava)

## Существуют ли в java многомерные массивы?
Многомерные массивы в их классическом понимании в java не существуют.
Многомерный массив всегда прямоугольный и неразрывен в памяти. А то, что в java считается мнгомерным - в других языках ещё называют "зубчатым массивом" или массивом массивов.
+ [Вопрос#21  К оглавлению](#ProceduralJava)

## Какими значениями инициируются переменные по умолчанию?
+ byte --> 0
+ short --> 0
+ int --> 0
+ long --> 0L
+ float --> 0.0f
+ double --> 0.0d
+ char --> '\u0000' 
+ boolean --> false
+ Обьекты --> null

Локальные (в методе) переменные не имеют значений по умолчанию, их имеют поля класса.
Не `static-поле` класса будет инициализировано после того, как будет создан объект этого класса. А `static-поле` будет инициализировано тогда, когда класс будет загружен виртуальной Java машиной.
+ [Вопрос#22  К оглавлению](#ProceduralJava)

## Что такое сигнатура метода?
__Это имя метода плюс параметры__ (порядок параметров имеет значение из-за множественной передачи данных через троеточие, которое должно располагаться последним). В сигнатуру метода не входит возвращаемое значение, а также бросаемые им исключения.
А сигнатура метода в сочетании с типом возвращаемого значения и бросаемыми исключениями называется __контрактом метода__.
+ [Вопрос#23  К оглавлению](#ProceduralJava)

## Расскажите про метод main
+ Является, как правило, точкой входа в программу и вызывается JVM. 
+ Как только заканчивается выполнение метода `main()`, так сразу же завершается работа самой программы.
+ `static` - чтобы JVM смогла загрузить его во время компиляции.
+ `public static void` и сигнатура - обязательное декларирование.
+ Мэйнов может быть много и может не быть вообще.
+ Может быть перегружен.

+ [Вопрос#24  К оглавлению](#ProceduralJava)

## Каким образом переменные передаются в методы, по значению или по ссылке?
__По значению!__ 
В случае с объектами, копируется и передается ссылка.
+ [Вопрос#25  К оглавлению](#ProceduralJava)

## Для чего используется оператор `assert`?
__Assert__ (Утверждение) — это специальная конструкция, позволяющая проверять предположения о значениях произвольных данных в произвольном месте программы. Утверждение может автоматически сигнализировать об обнаружении некорректных данных, что обычно приводит к аварийному завершению программы с указанием места обнаружения некорректных данных.

Утверждения существенно упрощают локализацию ошибок в коде. Даже проверка результатов выполнения очевидного кода может оказаться полезной при последующем рефакторинге, после которого код может стать не настолько очевидным и в него может закрасться ошибка. 

Обычно утверждения оставляют включенными во время разработки и тестирования программ, но отключают в релиз-версиях программ.

Т.к. утверждения могут быть удалены на этапе компиляции либо во время исполнения программы, они не должны менять поведение программы. Если в результате удаления утверждения поведение программы может измениться, то это явный признак неправильного использования _assert_. Таким образом, внутри _assert_ нельзя вызывать методы, изменяющие состояние программы, либо внешнего окружения программы. 

В Java проверка утверждений реализована с помощью оператора `assert`, который имеет форму:

`assert [Выражение типа boolean];` или `assert [Выражение типа boolean] : [Выражение любого типа, кроме void];`

Во время выполнения программы в том случае, если поверка утверждений включена, вычисляется значение булевского выражения, и если его результат `false`, то генерируется исключение `java.lang.AssertionError`. В случае использования второй формы оператора `assert` выражение после двоеточия задаёт детальное сообщение о произошедшей ошибке (вычисленное выражение будет преобразовано в строку и передано конструктору `AssertionError`).
+ [Вопрос#26  К оглавлению](#ProceduralJava)

## Какие логические операции и операторы вы знаете?
+ `&`: Логическое _AND_ (И);
+ `&&`: Сокращённое _AND_;
+ `|`: Логическое _OR_ (ИЛИ);
+ `||`: Сокращённое _OR_;
+ `^`: Логическое _XOR_ (исключающее _OR_ (ИЛИ));
+ `!`: Логическое унарное _NOT_ (НЕ);
+ `&=`: _AND_ с присваиванием;
+ `|=`: _OR_ с присваиванием;
+ `^=`: _XOR_ с присваиванием;
+ `==`: Равно;
+ `!=`: Не равно;
+ `?:`: Тернарный (троичный) условный оператор.

+ [Вопрос#27  К оглавлению](#ProceduralJava)


## Что такое тернарный оператор выбора?
Тернарный условный оператор `?:` - оператор, которым можно заменить некоторые конструкции операторов `if-then-else`.

Выражение записывается в следующей форме:
>условие ? выражение1 : выражение2

Если `условие` выполняется, то вычисляется `выражение1` и его результат становится результатом выполнения всего оператора. Если же `условие` равно `false`, то вычисляется `выражение2` и его значение становится результатом работы оператора. Оба операнда `выражение1` и `выражение2` должны возвращать значение одинакового (или совместимого) типа.
+ [Вопрос#28  К оглавлению](#ProceduralJava)

## Какие побитовые операции вы знаете?
+ `~`: Побитовый унарный оператор NOT;
+ `&`: Побитовый AND;
+ `&=`: Побитовый AND с присваиванием;
+ `|`: Побитовый OR;
+ `|=`: Побитовый OR с присваиванием;
+ `^`: Побитовый исключающее XOR;
+ `^=`: Побитовый исключающее XOR с присваиванием;
+ `>>`: Сдвиг вправо (деление на 2 в степени сдвига);
+ `>>=`: Сдвиг вправо с присваиванием;
+ `>>>`: Сдвиг вправо без учёта знака;
+ `>>>=`: Сдвиг вправо без учёта знака с присваиванием;
+ `<<`: Сдвиг влево (умножение на 2 в степени сдвига);
+ `<<=`: Сдвиг влево с присваиванием.

+ [Вопрос#29  К оглавлению](#ProceduralJava)

## Какие унарные и бинарные арифметические операции вы знаете?
Унарные операции выполняются над одним операндом, бинарные – над двумя операндами, а также тернарные – выполняются над тремя операндами. Операндом является переменная или значение (например, число), участвующее в операции.

Пример унарных арифметических операций:
+ / ++ – постфиксный/префиксный инкремент, увеличивает значение целочисленной переменной на 1;
+ / — (двойной минус) – постфиксный/префиксный декремент, уменьшает значение целочисленной переменной на 1;
+ / + – оставляет знак числа;
+ / – – изменяет знак числа.
Слово постфиксный означает, что операция применится к операнду после вычисления всего выражения, в которое операнд входит. Аналогично префиксный означает, что операция применится до вычисления выражения.

Пример бинарных арифметических операций:
+ / + – сложение чисел или строк;
+ / –  – вычитание чисел;
+ / * – умножения чисел;
+ / / – деления чисел;
+ / % – вычисление остатка от деления чисел.
Операция вычисления остатка от деления применима как к целым числам, так и к вещественным.

+ [Вопрос#30  К оглавлению](#ProceduralJava)

## Какова роль и правила написания оператора выбора (switch)?
Оператор switch сравнивает аргумент на равенство с предложенным значением.
```java
switch(ВыражениеДляСравнения) {
    case Совпадение1: 
	    команда;
		break;
	case Совпадение2: 
	    команда;
		break;
	case Совпадение3: 
	    команда;
		break;
	default: 
	    оператор;
	    break;
}
```
Обязательно необходимо ставить break; после завершения тело команды, иначе будет продолжаться выполнение ниже по строчкам.
Подробнее http://developer.alexanderklimov.ru/android/java/switch.php
+ [Вопрос#31  К оглавлению](#ProceduralJava)

## Какие циклы вы знаете, в чем их отличия?
В Java используются циклы for, while, do-while.
```java
while(условие) {
    // тело цикла
}
 
do {
    // тело цикла }
while(условие-логическое выражение)
 
for(инициализация; логическое выражение (условие); шаг (итерация)) {
    // тело цикла
}
 
for(Object object : objects) {
    // тело цикла 
}
```
do-while всегда выполнится хотя бы один раз, т.к. проверка идет после тела цикла.
+ [Вопрос#32  К оглавлению](#ProceduralJava)

## Какие операторы используются для перехода к следующей итерации и немедленной остановки цикла?
+ break; – выход из цикла (не затрагивает внешний цикл).
+ continue; – заканчивает выполнение кода в этом теле цикла. Переход к следующей итерации.
```java
for (int i=0; i < 3; i++) {
            for (int j = 0; j < 4; j++) {
                if (j == 2) {
                    System.out.println("#A# i: " + i + " j: " + j + " break (end j loop). Will not see #C#");
                    break;
                }
                if (j == 1) {
                    System.out.println("#B# i: " + i + " j: " + j + " continue (j++).Will not see #C#");
                    continue;
                }
                System.out.println("#C# i: " + i + " j: " + j);
            }
        }
#C# i: 0 j: 0
#B# i: 0 j: 1 continue (j++).Will not see #C#
#A# i: 0 j: 2 break (end j loop). Will not see #C#
#C# i: 1 j: 0
#B# i: 1 j: 1 continue (j++).Will not see #C#
#A# i: 1 j: 2 break (end j loop). Will not see #C#
#C# i: 2 j: 0
#B# i: 2 j: 1 continue (j++).Will not see #C#
#A# i: 2 j: 2 break (end j loop). Will not see #C#
```
+ [Вопрос#33  К оглавлению](#ProceduralJava)


## ССЫЛКИ НА ДОПОЛНИТЕЛЬНУЮ ИНФУ

+ [Название-->]( Ссылка )
+ [Название-->]( Ссылка )

+ [к оглавлению](#ProceduralJava)
