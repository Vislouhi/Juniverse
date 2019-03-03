## Switcher

### Переключатель.

#### Cинтаксис

    [switcher1]
    
    
#### Коментарий

     [//switcher1]
   
#### Пример

      [switcher1]
      switcherValues=[0,1,3,5]
      writeValueTo=state

   
#### Скрипты
     //Переключить switcher1 вперед
     {"Switcher":{"item":"1","action":"switchForward"}}
     //Переключить switcher1 вперед
     {"Switcher":{"item":"1","action":"switchBackward"}}





### Ключи

* switcherValues=[0,1]

Значения между которыми доступно переключение

* writeValueTo=state

Указывает в какую переменную записывать текущее значение 
