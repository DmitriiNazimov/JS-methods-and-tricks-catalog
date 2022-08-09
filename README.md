# Методы JS для работы со строками и массивами.

В данном конспекте отсутствует: 
- методы работы с юникодом.
- устаревшие (deprecated) и эксперементальные методы.

✅ - часто используемый метод, рекомендуется запомнить в первую очередь.

Конспект актуален по состоянию на август 2022 года.

## Оглавление
1. [Cоздание](https://github.com/NazimovDmitrii/JS-Array-and-String-methods/blob/main/README.md#%D1%81%D0%BE%D0%B7%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-%D0%BC%D0%B0%D1%81%D1%81%D0%B8%D0%B2%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%BA%D0%B8)

2. [Поиск](https://github.com/NazimovDmitrii/JS-Array-and-String-methods/blob/main/README.md#%D0%BF%D0%BE%D0%B8%D1%81%D0%BA-%D0%BF%D0%BE-%D0%BC%D0%B0%D1%81%D1%81%D0%B8%D0%B2%D1%83%D1%81%D1%82%D1%80%D0%BE%D0%BA%D0%B5)

3. [Извлечение](https://github.com/NazimovDmitrii/JS-Array-and-String-methods/blob/main/README.md#%D0%B8%D0%B7%D0%B2%D0%BB%D0%B5%D1%87%D0%B5%D0%BD%D0%B8%D0%B5-%D0%B8%D0%B7-%D0%BC%D0%B0%D1%81%D1%81%D0%B8%D0%B2%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%BA%D0%B8)

4. [Проверка по условию](https://github.com/NazimovDmitrii/JS-Array-and-String-methods/blob/main/README.md#%D0%BF%D1%80%D0%BE%D0%B2%D0%B5%D1%80%D0%BA%D0%B0-%D0%BF%D0%BE-%D1%83%D1%81%D0%BB%D0%BE%D0%B2%D0%B8%D1%8E--%D1%81%D1%80%D0%B0%D0%B2%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5)

5. [Простое преобразование](https://github.com/NazimovDmitrii/JS-Array-and-String-methods/blob/main/README.md#%D0%BF%D1%80%D0%BE%D1%81%D1%82%D0%BE%D0%B5-%D0%BF%D1%80%D0%B5%D0%BE%D0%B1%D1%80%D0%B0%D0%B7%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5-%D0%B1%D0%B5%D0%B7-%D0%BA%D0%BE%D0%BB%D0%BB%D0%B1%D1%8D%D0%BA%D0%B0)

6. [Сложное преобразование](https://github.com/NazimovDmitrii/JS-Array-and-String-methods/blob/main/README.md#%D1%81%D0%BB%D0%BE%D0%B6%D0%BD%D0%BE%D0%B5-%D0%BF%D1%80%D0%B5%D0%BE%D0%B1%D1%80%D0%B0%D0%B7%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5-%D1%81-%D0%BA%D0%BE%D0%BB%D0%BB%D0%B1%D1%8D%D0%BA%D0%BE%D0%BC)

## Создание массива/строки

### Массив
 - ✅ [String.**split**(separator)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split) - создает МАССИВ путем разбиения String на подстроки по разделителю separator.

- []() - 

- []() - 

- []() - 

- []() - 

- []() - 

- []() - 

### Строка
❌ - [String.**raw**()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/raw) - создает строку которая вставляется как `Some text ${string}` и в ней спецсимволы типа u000A не исполняются. Грубо говоря экранирует спецсимволы.


## Поиск по массиву/строке

### Массив
- [Array.**find**(callback(item, index, arr)) | **.findLast**()](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/find) - возвращает **значение** первого/последнего найденного в массиве элемента, которое удовлетворяет условию переданному в callback функции. В противном случае возвращается undefined.

- [Array.**findIndex**(callback(item, index, arr)) | **.findLastIndex**()](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/findIndex) - возвращает **индекс** первого/последнего элемента в массиве, если элемент удовлетворяет условию проверяющей функции. В противном случае возвращается -1.

- []() - 

- []() - 

### Строка
- ✅ [String.**search**(regex)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/search) - возвращает индекс первого вхождения regex в строку String или -1 если вхождения нет. 

- ✅ [String.**indexOf**('sample') | **lastIndexOf**()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/indexOf) - возвращает индекс первого/последнего вхождения указанной подстроки.

- ✅ [String.**includes**('sample')](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/includes) - определяет с учетом регистра присутствует ли 'sample' внутри String. Возвращает true/false.

- [String.**startsWith**('sample') | **endsWith**('sample')](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/startsWith) - определяет есть ли в начале/конце строки String строка 'sample'. Возвращает true/false.

## Извлечение из массива/строки

### Массив
- [Array.**at**(index)](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/at) - возвращает элемент массива по index. В отличие от квадратных скобок работает с отрицательными числами. Например Array.at(-1) вернет последний элемент массива.

- []() - 

- []() - 

- []() - 

- []() - 

- []() - 

- []() - 

### Строка
- ✅ [String.**slice**(indexStart, indexEnd)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/slice) - извлекает часть строки и возвращает ее как новую строку без изменения исходной строки.

- ✅ [String.**match**(regexp) | **matchAll**(regexp)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/match) - извлекает из строки символы по условию regexp. Возвращает массив извлеченных символов.

- [String.**substring**(indexStart, end)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/substring) - возвращает часть string между начальным и конечным индексами? или до конца строки.

- [String.**charAt**(index)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/charAt) - извлекает 1 символ по номеру его индекса в строке. Возвращает 1 символ.



## Проверка по условию | сравнение

### Массив
- [Array.**every**(callback(item, index, arr) | .**some**())](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/every) - проверяет, удовлетворяют ли все/некоторые элементы массива условию, заданному в передаваемой функции. Возвращает true/false.

- []() - 

- []() - 

- []() - 

### Строка
- [String.**localeCompare**(compareString, locales, options)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/localeCompare) - сравнение строк. Возвращает -1, 0 или 1. 0 - означает равенство. 




## Простое преобразование (без коллбэка)

### Массив
- [Array.**concat**(anotherArr)](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/concat) - возвращает новый массив, состоящий из массива, на котором он был вызван, соединённого с другими массивами.
 
- [Array.**copyWithin**(target, start, end)](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/copyWithin) - копирует последовательность элементов массива внутри него в позицию, начинающуюся по индексу target. [1, 2, 3, 4, 5].copyWithin(0, 3); // [4, 5, 3, 4, 5] // Вставляет с элемента ноль элементы с 3 до последнего.
 
- [Array.**entries**()](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/entries) - возвращает новый объект итератора массива Array Iterator, содержащий пары ключ / значение для каждого индекса в массиве.

- [Array.**fill**(value, start, end)](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/fill) - заполняет все элементы массива от начального до конечного индексов одним значением. Возвращает измененный массив.

- []() - 

- []() - 

- []() - 

- []() - 

### Строка
- ✅ [String.**replace**(regexp, newSubstr) | **replaceAll**(regexp, newSubstr)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/replace) - возвращает новую строку, в которой заменяет в строке String одно вхождение найденное по regexp на newSubstr.

- ✅ [String.**toLowerCase**() | **toUpperCas**e()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/toLowerCase) - возвращает новую строку преобразованную в нижний/верхний регистр.

- ✅ [String.**trim()** | trimEnd() | trimStart()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/Trim) - удаляет пробелы с обоих концов строки и возвращает новую строку без изменения исходной строки. 

- [String.**concat**()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/concat) - обьединяет строки и возвращает новую объединенную строку.

- [String.**padEnd**(length, 'sample')](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/padEnd) - добавляет в конец текущей строки подстроку "sample", чтобы результирующая строка достигла заданной длины length.

- [String.**padStart**(length, 'sample')](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/padStart) - добавляет в начало текущей строки подстроку "sample", чтобы результирующая строка достигла заданной длины length.

- [String.**repeat**(5)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/repeat) - возвращает новую строку, указанное количество раз копируется эта же строка.


## Сложное преобразование (с коллбэком)

### Массив
- [Array.**filter**(callback(item, index, array))](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/filter) - создаёт новый массив со всеми элементами, прошедшими проверку, задаваемую в передаваемой функции.

- []() - 

- []() - 
