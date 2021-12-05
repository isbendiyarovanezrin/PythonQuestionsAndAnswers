<div align="center">
  <img width="65" src="https://i.postimg.cc/50RBRxjd/python.png">

### **Python Interview Questions and Answers**

</div>
<br>

1.  #### **What is the built-in function used in Python to iterate over a sequence of numbers?**

    Pythonda **range()** funksiyası ədədlər ardıcıllığını qaytarır və default olaraq 1-dən başlayır, 1-1 artır və müəyyən edilmiş ədəddən sonra dayanır.

    Sintaksisi bu şəkildədir: **range(start, stop, step)**

    _Nümunə:_

    ```py
    for n in range(5, 12):
      print (n)
    ```

    Bu zaman ardıcıllıq 5-dən başlayıb (5 də daxil olmaqla) 12-yə qədər (12 daxil deyil) davam edəcək.

    _Çıxış:_

    ```
    5
    6
    7
    8
    9
    10
    11
    ```

    _Başqa bir nümunəyə baxaq:_

    ```py
    for i in range(2, 15, 3):
      print (i)
    ```

    Ardıcıllıq 2-dən başlayıb 15-ə qədər 3-3 artaraq davam edəcək.

    _Çıxış:_

    ```
    2
    5
    8
    11
    14
    ```

<br>

2. #### **Suppose list1 is [2, 12, 222, 55, 52]. What is list1[-1]?**
   Ədəd mənfi (sondan başlayacaq) və 1 (1-ci ədədi götürəcək) olduğu üçün cavab 52 olacaq.

<br>

3. #### **Explain the //, %, and \*\* operators in Python.**

   `//` operatoru qalıqsız bölmə operatorudur. Nəticə həmişə tam ədəd olur. <br>

   _Nümunə:_

   ```py
   55 // 10
   ```

   5 qaytaracaq, çünki 55-in içində 5 dənə 10 var. Qalıq isə nəzərə alınmır. Əgər adi bölmə əməliyyatı (55 / 10) ilə yazsaydıq cavab 5.5 olardı.

   <br>

   `**` operatoru qüvvətə yüksəltmə operatorudur. <br>

   _Nümunə:_

   ```py
   5 ** 2
   ```

   25 qaytaracaq, çünki 5-i 2 dəfə öz-özünə vuranda (5 üstü 2) 25 edir.

   <br>

   `%` operatorunun mənası budur ki, məsələn, a b-yə bölünür və onların bölünməsindən qalıq c alınır. Buradakı qalıq c `a % b` ifadəsinin cavabıdır.

   _Nümunə:_

   ```py
   50 % 12
   ```

   2 qaytaracaq, çünki 50 12-yə bölünür və cavab 4 (qalıq 2) olur. Qalıq 2 olduğu üçün də cavab 2 olacaq.

<br>

4. #### **Explain logical operators in Python.**

   Məntiqi operatorlar şərti ifadələrdə istifadə olunur və boolean dəyər (True və ya False) qaytarır. Pythonda 3 məntiqi operator var.

   | Operator |                                       Təsviri                                       | Sintaksisi |
   | :------: | :---------------------------------------------------------------------------------: | :--------: |
   |   and    |                     Əgər hər iki tərəf doğrudursa True qaytarır                     |  a and b   |
   |    or    |                   Əgər iki tərəfdən biri doğrudursa True qaytarır                   |   a or b   |
   |   not    | Nəticəni tərsinə çevirir, əgər doğrudursa False qaytarır, yanlışdırsa True qaytarır |   not a    |

   _Nümunə:_

   ```py
   a = 5

   print(5 >= a and 20 > a) # True qaytarır, çünki şərtlərin hər ikisi də doğrudur

   print(5 < a or 20 > a) # True qaytarır, çünki şərtlərdən biri doğrudur

   print(not(5 < a or 20 > a)) # False qaytarır, çünki nəticə tərsinə çevrilir
   ```

   Belə bir cədvəllə sualı yekunlaşdıraq.

   | Operator A | Operator B | Logical AND nəticə |
   | :--------: | :--------: | :----------------: |
   |    True    |    True    |        True        |
   |    True    |   False    |       False        |
   |   False    |    True    |       False        |
   |   False    |   False    |       False        |

   | Operator A | Operator B | Logical OR nəticə |
   | :--------: | :--------: | :---------------: |
   |    True    |    True    |       True        |
   |    True    |   False    |       True        |
   |   False    |    True    |       True        |
   |   False    |   False    |       False       |

   | Operator A | Logical NOT nəticə |
   | :--------: | :----------------: |
   |    True    |       False        |
   |   False    |        True        |

   <br>

5. #### **How do you calculate the length of a string?**

   Bunun üçün **len()** funksiyasından istifadə edirik və string'lərin uzunluğunu hesabladığımız üçün nəticə olaraq xarakterlərin sayını qaytarır.

   _Nümunə:_

   ```py
   s = len("mətn")
   print(s) # 4 qaytarır

   a = len("Salam, Zöhrab!")
   print(a) # 14 qaytarır
   ```
