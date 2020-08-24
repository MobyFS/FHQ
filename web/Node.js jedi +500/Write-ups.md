## Задача: 
    EN
    Get access to secret information
    http://fhq2015-500-nodejs-jedi.freehackquest.com

    RU
    Получить доступ к секретной информации
    http://fhq2015-500-nodejs-jedi.freehackquest.com


## Ответ:
    fhq2015{Ride_The_Lightning}

## Автор: 
    [keva] Nitive

## Разбор:
    1. Делаем попытку захода на http://fhq2015-500-nodejs-jedi.freehackquest.com/package.json (почему именно туда? Он практически всегда присутсвует в проектах использующие node.js)

    2. Сразу же выделяем нужную нам информацию: "description": "Service for FHQ 2015. See README.md for additional information",

    3. Переходим в README.md точно таким же образом

    4. Внутри README.md видим инструкцию, и исходя из неё,вытаскиваем еще 1 файл и страничку: index.coffee (страничка) start.sh (файл) и (точно таким же образом как и ранее) 

    5. Сразу же в глаза бросается ошибка в файле start.sh: ADMIN_PAS, а должно быть ADMIN_PASS

    6. Далее анализирует index.coffee и замечаем следующее: в "process.env.ADMIN_PASS" стоит undefined, что нам это говорит? Что это эквивалентно записи #{process.env.ADMIN_PASS} === 'undefined', следовательно подставляя undefined в пароль мы получаем доступ к админке. 
    
    7. Заходим в админку и получаем наш флаг: Ride_The_Lightning