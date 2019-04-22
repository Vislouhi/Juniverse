## Cylinder

### Отображает 3D модель цилиндра

#### Cинтаксис

    [cylinder1]
    
    
#### Коментарий

     [//cylinder1]
   
#### Пример

    [cylinder1]
    startPosition={"x":"csX","y":"csY","z":"csZ"}
    endPosition={"x":"pointerX","y":"pointerY","z":"pointerZ"}
    color={"r":"1","g":"1","b":"0","a":"0.5","reflection":3,"specularStrength":1}
    edges=4
    radius=0.03

#### Скрипты
        [script(example)]
        //Включить и выключить отображение цилиндра
        {"Cylinder":{"item":1,"visible":"on"}}
        {"Cylinder":{"item":1,"visible":"off"}}
       


### Ключи

* startPosition={"x":"csX","y":"csY","z":"csZ"}

Начальная точка цилиндра, может быть задана числом или формулой

* endPosition={"x":"pointerX","y":"pointerY","z":"pointerZ"}

Конечная точка цилиндра, может быть задана числом или формулой

* color={"r":"1","g":"1","b":"0","a":"0.5","reflection":3,"specularStrength":1}

Параметры материала цилиндра

* edges=4

Количество ребер цилиндра

* transperencyOrderIndex = 1

Индекс указывает в какой последовательности осуществлять рендеринг прозрачных объектов

* radius=0.03

Радиус цилиндра
