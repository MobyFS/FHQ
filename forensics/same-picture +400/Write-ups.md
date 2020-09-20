## Задача: 

    RU: Сегодня всем пришла одна и та же картинка. Что тут не так? Подсказка: Где то это уже было... поломай себе мозг

    EN: Today all came the same picture. What's wrong here? Hint: Where it was already broken their brains ...

## Ответ:
    revival_of_the_cicada

## Автор: 
    [LiFe] by.smirnowmaks

## Разбор:
    1. Смотрим что находится внутри этой ути, binwalk <filename>
    2. Видим,что там есть какой-то архив,достаем его binwalk --dd='.*' <filename>
    3. В архиве находим файл 0.txt, внутри нас ожидает brainfuck 
    4. Декодим brainfuck и получаем подскажу в виде: password - cicada programm - outguess
    5. Пользуясь данной подсказкой юзаем outguess и достаем информацию которая скрыта в нашей уте: outguess -k cicada -r DFDE72D3-5BF5-0216-A80A-AF3FFB705515_forenzika_400_111.jpg test.txt (не забудь поменять формат файла на .jpg,а то outguess тебя пошлет куда подальше)
    6. Поздравляю ты получил флаг!
