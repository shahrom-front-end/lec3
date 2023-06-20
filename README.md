# lec3

## Метод — это блок кода, который запускается только при вызове.Вы можете передавать данные, известные как параметры, в метод.Методы используются для выполнения определенных действий, и они также известные как функции.

## мо 3 намуди сохтани стринг дорем

```js
  1  let a="Hello"
```
```js
  2  let a='Hello'
```
```js
  3  let a=`Hello${hi}`
```

# 1 JavaScript метод charAt() возвращает символ по заданному индексу внутри строки. Индекс первого символа равен нулю, а последнего рассчитывается как значение длины строки - 1 ( length - 1 ). 
```js
    let str1="my name is Shahrom"
    let str2=str1.charAt(11)
    console.log(str2);//S
```
# 2 Метод concat создаёт новый массив, состоящий из элементов в объекте, на котором он был вызван, за которыми по порядку следуют, для каждого аргумента, все его элементы (если аргумент является массивом), либо сам аргумент (если он массивом не является).Метод concat не изменяет данный массив или любой из массивов, переданных в аргументах, а вместо этого возвращает поверхностную копию, содержащую копии тех элементов, что были объединены с исходными массивами. Элементы оригинальных массивов копируются в новый массив по следующим правилам

```js
    let str1="my name is Shahrom"
    let str2="hello"
    let str3=str1.concat(" ",str2)
    console.log(str3);//my name is Shahrom hello
```

# 3 Метод replace() возвращает новую строку с некоторыми или всеми сопоставлениями с шаблоном, заменёнными на заменитель. Шаблон может быть строкой или регулярным выражением, а заменитель может быть строкой или функцией, вызываемой при каждом сопоставлении
```js
    let str1="in the softclub main";
    let str2=str1.replace("the","turbo");
    console.log(str2);//in turbo softclub main
```

# 4 Метод replaceAll() возвращает новую строку со всеми совпадениями pattern , который меняется на replacement . pattern может быть строкой или регулярным выражением, и replacement может быть строкой или функция возвращающая каждое совпадение. Исходная строка остаётся без измененийд
 ```js
    let str1="in the softclub main the moon the";
    let str2=str1.replaceAll("the","turbo");
    console.log(str2);//in turbo softclub main turbo moon turbo
```

# 5 Метод split() разбивает объект String на массив строк путём разделения строки указанной подстрокой
```js
let str1="softclub"
let str2=str1.split("")
console.log(str2)  //['s', 'o', 'f', 't', 'c', 'l', 'u', 'b']
```

# 6 Метод substring() возвращает подстроку строки между двумя индексами, или от одного индекса и до конца строки
```js
    let str1="softclub"
    let str2=str1.substring(2)
    console.log(str2)// ftclub

    let str1="softclub"
    let str2=str1.substring(2,4)
    console.log(str2)// ft
```

# 7 Метод slice() возвращает новый массив, содержащий копию части исходного массива
```js
    let str1="text align center"
    let str2=str1.slice(2)
    console.log(str2);//xt align center
    
    let str1="text align center"
    let str2=str1.slice(2,10)
    console.log(str2);//xt align
```

# 8 Метод toLowerCase() возвращает значение строки, на которой он был вызван, преобразованное в нижний регистр
```js
    let str="YOU DED"
    let str2=str.toLowerCase()
    console.log(str2);//you ded
```
# 9 Метод toUpperCase() возвращает значение строки, преобразованное в верхний регистр
```js
    let str="you ded"
    let str2=str.toUpperCase()
    console.log(str2);//YOU DED
```

# 10 Метод trim() удаляет пробельные символы с начала и конца строки. Пробельными символами в этом контексте считаются все собственно пробельные символы (пробел, табуляция, неразрывный пробел и прочие) и все символы конца строки (LF, CR и прочие)
```js
    let str="        you ded          "
    let str2=str.trim()
    console.log(str2);//"you ded"
```
# 11 Метод includes() определяет, содержит ли массив определённый элемент, возвращая в зависимости от этого true или false

```js
    let str="you ded"
    let str2=str.includes("ded")
    console.log(str2);//true

    let str="you ded"
    let str2=str.includes("moon")
    console.log(str2);//false
```

# 12 Метод toString() преобразует объект в строковое представление. Метод автоматически вызывается JavaScript, когда объект нужно представить в текстовом виде. Если метод не переопределён, то он возвращает строку формата [object тип] , где тип — это строка, которая уточняет тип объекта
```js
    let str=2+2
    let str2=str.toString()
    console.log(typeof(str2));//string

    let str=2+2
    let str2=str.toString()
    console.log(`hello ${str2}`);//"hello 4"
```

# 13 Метод indexOf() возвращает индекс первого вхождения указанного значения в строковый объект String , на котором он был вызван, начиная с индекса fromIndex 
```js
    let str="my name  is Shahrom"
    let str2=str.indexOf("is")
    console.log(str2);//index 9
```

# 14 repeat() Метод repeat() конструирует и возвращает новую строку, содержащую указанное количество соединённых вместе копий строки, на которой он был вызван
```js
    let str="Shahrom"
    let str2=str.repeat(2)
    console.log(str2);//"ShahromShahrom"
```

# 15 Метод at() является эквивиалентом получения элементов массива с помощью квадратных скобок с использованием неотрицательного индекса
```js
    let str="Shahrom"
    let str2=str.at(2)
    console.log(str2);//"a"

    let str="Shahrom"
    let str2=str.at(-2)
    console.log(str2);//"o"
```
# -----------------------------------------------------------
                                # JavaScript Number methods 

# 1 Метод Math.round() возвращает число, округлённое к ближайшему целому
```js
    let n=3.8
    let n1=Math.floor(n)
    console.log(n1);// 3
```
# 2 Сводка Метод Math. ceil() - округление вверх. Округляет аргумент до ближайшего большего целого.

```js
    let n=3.3
    let n1=Math.ceil(n)
    console.log(n1);// 4
```

# 3 Метод Math.round() возвращает число, округлённое к ближайшему целому
```js
    let n=3.3
    let n1=Math.round(n)
    console.log(n1);// 3

    let n=3.6
    let n1=Math.round(n)
    console.log(n1);// 4
```
# 4 Метод Math. max() возвращает наибольшее из нуля или более чисел
```js
    let n1=23
    let n2=12
    let n3=32
    let result=Math.max(n1,n2,n3)
    console.log(result);// 32
```
# 5 Метод Math. min() возвращает наименьшее из нуля или более чисел
```js
    let n1=23
    let n2=12
    let n3=32
    let result=Math.min(n1,n2,n3)
    console.log(result);// 12
```
# 6 Метод Math. pow() возвращает основание , возведённое в степень показатель , то есть, значение выражения основаниепоказатель .
```js
    let result=Math.pow(5,3)
    console.log(result);//125
```

# 7 Квадратный корень заданного числа.
```js
    let result=Math.sqrt(16)
    console.log(result);//4
```

# 8 Этот метод возвращает абсолютное значение числа, то есть иными словами - если число неотрицательное, то его и возвращает, а если отрицательное - отбрасывает знак "минус"
```js
    let n=-16
    let result=Math.abs(n)
    console.log(result);//16
```
# 9 Метод Math. random() возвращает псевдослучайное число с плавающей запятой из диапазона (0, 1) , то есть, от 0 (включительно) до 1 (но не включая 1), которое затем можно отмасштабировать до нужного диапазона
```js
    let result=Math.random()
    console.log(result);//0.015841437065600372

    let result=Math.random()*10
    console.log(result);//7.198228262115087
```

# 10 Функция isNaN() определяет является ли литерал или переменная нечисловым значением ( NaN ) или нет. При работе с функцией необходимо проявлять осторожность так как она имеет свои особенности. В качестве альтернативы можно использовать метод Number
```js
    let n="fd"
    console.log(isNaN(n));// true

    let n=12
    console.log(isNaN(n));// false
```
# banana

```js
    let ded=("b"+ "a"+ +'a'+'a').toLowerCase()
    console.log(ded);//banana
```

