# Ячейки (cell), массивы ячеек

Ячейка(cell) - контейнер, который может содержать в себе объект произвольного типа данных
(т.е. это может быть массив чисел с плавающей запятой, массив символов, массив структур и др.) 

Массив ячеек — это коллекция ячеек, доступ к которым происходит по индексу. Таким образом, массив ячеек может объединять разнотипные данные. Массив может быть одномерным, двумерным или многомерным. 

Элементом массива ячеек может быть ячейка и массив ячеек.

Доступ к ячейкам осуществляется указанием после имени массива индекса элемента в фигурных скобках.

Например:

Чтобы создать массив пустых ячеек достаточно воспользоваться функцией cell с указанием размеров массива:

  M = cell(5, 2, 3)
  
Так же можно создать массив ячеек и сразу инициализировать его:

  с = {1 'a' 'Ivan' 2834 ; 'b' 6 14:19 29}
  
  c = 

    [1]    'a'    'Ivan'          [2834]
    'b'    [6]    [1x6 double]    [  29]
    
  Обращение к элементам массива такое же, как и к элементам обычного массива. При этом получаем ячейку:
   
    с(2,3)
      ans = 

         [1x6 double]
         
  Для извлечения содержимого ячейки нужно использовать {}:
  
  c{2,3}

  ans =

    14    15    16    17    18    19
    
  При обращении к содержимому массива и ячеек можно использовать end:
  
  c(2:end)

  ans = 

      'b'    'a'    [6]    'Ivan'    [1x6 double]    [2834]    [29]
      
      
  c{2:end}

    ans =

        b


    ans =

        a


    ans =

        6


    ans =

        Ivan


    ans =

        14    15    16    17    18    19


    ans =

        2834


    ans =

        29
  
