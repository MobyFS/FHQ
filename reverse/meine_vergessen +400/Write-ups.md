## Задача: 

    EN: What say foxes? RU: Что говорят лисы?

    Hint 1. Strings could not help you

## Ответ:
    foxes5ayHumansMu5tD1e

## Автор: 
    [keva] sea-kg

## Разбор:
    1. Открываем exe в условном dotPeek и чекаем код

    2. Замечаем,что у нас есть некий статический "массив" (это не совсем массив,называю так для общего понимания) символов 
        private static string chars = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789";

    3. В функции buttonGenerate_Click видим условие 
        "if (this.m_textPassword.Text == this.getPassword())
            this.m_textNewPassword.Text = this.getNewPassword();"
        Это определенно то что нам нужно! Осталось заставить программу выполнить эти условия 
    
    4. Идем в функцию getPassword и внимательно читаем данную функцию, видим там следующее:
        "MyPassword.chars[38],
        MyPassword.chars[24],
        MyPassword.chars[this.getChar("6")],
        MyPassword.chars[this.getChar("8")],
        MyPassword.chars[this.getChar("c")],
        MyPassword.chars[this.getChar("R")],
        MyPassword.chars[this.getChar("e")],
        MyPassword.chars[this.getChar("7")],
        MyPassword.chars[this.getChar("P")],
        MyPassword.chars[this.getChar("2")]"
        Видно,что первые два символа берутся из того самого "массива" 
    
    5. Вводим эту последовательность и получаем флаг 
