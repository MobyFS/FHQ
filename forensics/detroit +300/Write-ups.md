## Задача: 

    RU: Представте себе что у вас имеется БД сотрудников одной крупной корпорации, отделения которой, разбросанной по всей Северной Америке. Нужно найти чувака, но точно о нем мало известно. Зовут его вроде Вилл, а может и нет, он связан с безопасностью в этой корпорации. Еще известно что он работает в детройском отделении.

    EN: Imagine that you have a database of employees of a major corporation, with offices scattered throughout North America. We need to find the guy, but I do know about it a little. His name is like Will, but maybe not, it is associated with security in this corporation. Even know that it works in the Detroit office.

    Hint: pass

## Ответ:
    Yeap_th1s_pss

## Автор: 
    [keva] f0x3

## Разбор:
    1. Очень внимательно читаем описание и из него делаем вывод,что человека которого мы ищим зовут William и он занимается безопасностью. 
    2. Грепаем всех Виллов и далее смотрим на их они занимаются в данной компании
    3. Грепаем все ИБшные должности,далее сортируем их и отбираем
    4. Натыкаемся на некого William Polk,берет оттуда Crypto pass WWVhcF90aDFzX3Bzcw== (очевидно,что это base64)
    5. Декодируем 
    6. Получаем флаг Yeap_th1s_pss
