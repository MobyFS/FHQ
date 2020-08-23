## Задача: 

    <?php
	if (md5($code) == md5('240610708') && $code != '240610708'){
		print $flag;
		exit();
	}
	?>

## Ответ:
    QNKCDZO

## Автор: 
    [life] by_sm

## Разбор:
    Все очень легко, это просто коллизия MD5
    Можете почитать тут: https://ru.wikipedia.org/wiki/MD5#Коллизии_MD5
