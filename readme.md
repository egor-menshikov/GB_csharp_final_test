Задача: Написать программу, которая из имеющегося массива строк формирует новый массив из строк, длина которых меньше, либо равна 3 символам. Первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма. При решении не рекомендуется пользоваться коллекциями, лучше обойтись исключительно массивами.

### Решать буду так:

* Три проверочных массива задам сам.

* Блок-схему делаю для основного метода в котором происходит решение.

* Будет два метода: метод на вывод массива на экран и рабочий метод.

___Что будет происходить в рабочем методе:___

1) Он принимает один string[] массив, работает, и выдает другой. 

2) Сначала он считает количество элементов во входном массиве длиной 3 или менее символа, и записывает их в переменную count.

3) Затем создает string[] массив длиной count.

4) Цикл в цикле - внешний проходит по элементам нового массива чтобы записывать в них значения из старого, которые нам подходят по количеству символов.

5) Внутренний будет искать по элементам старого цикла подходящие нам элементы для записи. Начинать он будет с j = i + shift. Здесь мы стартуем с i для того, чтобы не записывать уже найденные до этого элементы. Также мы используем переменную "сдвига" shift, которую будем увеличивать на 1 каждый раз когда видим неподходящий нам элемент. Таким образом мы учитываем и те элементы которые уже записаны, и те, которые нам не подходят. 

6) Как только мы находим подходящий элемент мы его копируем в новый массив и прерываем внутренний цикл чтобы избежать перезаписи в этот конкретный индекс i.

### Все
* Дальше просто показываю по очереди входной массив, и массив который получился в результате работы программы, для всех трех входных массивов.


