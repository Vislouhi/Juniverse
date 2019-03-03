## LcdDisplay

### Отображает 3D модель на экране

#### Cинтаксис

    [lcdDisplay1]
    
    
#### Коментарий

     [//lcdDisplay1]
   
#### Пример

    [lcdDisplay1]
    position={"x":"1","y":"2","z":"2+sin(alpha)"}
    rotation={"x":"1.0","y":"0.0","z":"0.0","angle":"alpha*0.5"}
    rotationXYZ ={"x":"0","y":"0.5","z":"-0.5"}
    scale=0.5
    texturePack=calc
    value=pointerX

#### Скрипты
        [script(example)]
        //Включить и выключить отображение цифр
        {"LcdDisplay":{"state":"on"}}
        {"LcdDisplay":{"state":"off"}}
       


### Ключи


* position={"x":"1","y":"2","z":"2+sin(alpha)"}

Позиция объекта, может быть задана числом, или формулой

* rotation={"x":"1.0","y":"0.0","z":"0.0","angle":"alpha*0.5"}

Поворот объекта.

x,y,z - направление оси, вокруг которой совершается поворот

angle - угол поворота в радианах

* rotationXYZ ={"x":"0","y":"0.5","z":"-0.5"}

Поворот объекта вокруг осей XYZ  на соответствующие углы

* scale=0.5

Масштаб объекта

* texturePack=calc

В качестве цифр будут загружены картинки типа png

calc0.png, calc1.png ... calc13.png , calcBlanc.png, calcDot.png, calcNoDot.png

* value=pointerX

Число, которое выводится на табло, может быть задано формулой
