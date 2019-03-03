## TriggerPoint

### Датчик пространственного обнаружения объекта Item. 

#### Cинтаксис

    [triggerPoint1]
    
    
#### Коментарий

     [//triggerPoint1]
   
#### Пример

    [triggerPoint1]
    availableItems=[1,2,3]
    onContact=2
    position={"x":"0.0+mainX","y":"-1.5+mainY","z":"-1.0+mainZ"}
    radius=0.3








### Ключи
[triggerPoint1]

* availableItems=[1,2,3]

* availableItems=["i1","i2","i3"]

Доступные для проверки объекты item

* onContact=2

Указывает какой скрипт будет выполнен при контакте

* position={"x":"0.0+mainX","y":"-1.5+mainY","z":"-1.0+mainZ"}

Позиция триггерной точки может быть задана числом или формулой

* radius=0.3
