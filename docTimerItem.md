## TimerItem

### Таймер

#### Cинтаксис

    [timerItem1]
    
    
#### Коментарий

     [//timerItem1]
   
#### Пример

    [timerItem1]
    startAt=0.0
    writeValueTo=timerValue
    
#### Скрипты   
    //Включить timerItem1 и сбросить значение.
    {"TimerItem":{"item":"1","state":"on","resetTo":"0"}}}

### Ключи

* startAt=0.0

Начинать отсчет с заданного значения

* writeValueTo=timerValue

Писать время в указанную переменную
