## Задача: 

    You work for FBI and you need to hack this file from Columbian Bank...

## Ответ:
    309f5933b45a8e31074a9e04f8905349

## Автор: 
    user0

## Разбор:
    1. Открываем в IDA 

    2. Далее можно рассмотреть несколько вариантов решения этого таска, мы рассмотрим самый простой, пропатчим

    3. Из адреса loc_401062 переходим напрямую в loc_401112 (jmp short loc_401112)

    4. Видим еще одно разветвление,нам нужно попасть в ветку с "Yep! You win! Take a flag\n Flag = ", для этого мы в адресе loc_401112 патчим jnz на jne

    5. Сохраняем наш пропатченный файл 

    6. Запускаем файл в расширении "exe", вводим "1" и получаем флаг :)
