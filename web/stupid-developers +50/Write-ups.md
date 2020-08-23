## Задача: 
    Stupid Developers...
    Stupid Developers...
    Stupid Developers...
    Stupid Developers...
    Глупые разработчики...

    [here index.php](https://freehackquest.com/files/quests/78B7FDBD-D781-8DF5-1670-4988282C623A_index.php)

## Ответ:
    very-hard-pass

## Автор: 
    [keva] sea-kg

## Разбор:
    1.Открываем код страницы
    2.Пролистав немного вниз,обнаруживаем javascrip, раскрываем и видим две функции
    3.Проведя анализ понимаем,что первая функция занимается декодом,а вторая содержит очень интересную строчку:
    
    if(val == 'e4bcb6aa3a34fde3ef4e95446ebc9422')
    
    4.Пробуем ввести это на страничке (e4bcb6aa3a34fde3ef4e95446ebc9422)
    5.Получаем флаг: very-hard-pass