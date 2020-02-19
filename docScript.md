## Script

### Выполнение действий для объектов

#### Cинтаксис

    [script1]
    
    или
    
    [script(newScript)]
    
    
    
#### Коментарий

     [//script1]
   
#### Пример

    [script(newScript)]
    {"setVariables":{"dH":"0.001"}}
    {"RigidBody":{"item":"1", "x":"oX","y":"oY-0.5","z":"oZ"}}
    //Выполнить скрипт при условии dH<10
    {"RigidBody":{"condition":{"dH":"<10"},"item":"1", "x":"oX","y":"oY-0.5","z":"oZ"}}
    
#### Скрипты
        //Выполнить скрипт в этом узле
       {"Script":{"execute":"script"}}
       //Выполнить скрипт в узле "start"
       {"Script":{"node":"start","execute":"script"}}
       //Выполнить скрипт в этом узле с задержкой в 2с
       {"Script":{"execute":"script","delay":"2"}}
    

### Скрипты не относящиеся к объектам

* Присвоить значение переменной

      {"setVariables":{"a":"1"}}
      
      или
      
      {"setVariables":{"a":"1+cos(x)"}}

* Задать растояние от указателя до точки обзора
  
      {"Pointer3D":{"length":"1.5"}}
      
 ### Выполнение скрипта по условию    
 
         {"setVariables":{"condition":{"a":"<9","b":"=0","c":">3","d":"!3"},"a":"a+1","b":"1"}}
 
  ### Особые переменные
  
  * pointerX, pointerY, pointerZ - координаты указателя
   
         //Присвоить переменным x, y, z координаты указателя, соответственно. 
         {"setVariables":{"x":"pointerX","y":"pointerY","z":"pointerZ"}}  
       
 * positionX, positionY, positionZ - положение камеры
 
       //(x, y, z) -вектор с направлением обзора 
       {"setVariables":{"x":"pointerX-positionX","y":"pointerY-positionY","z":"pointerZ-positionZ"}}  
    
  * cameraAngleX, cameraAngleY - углы поворота камеры
  
  
  * random - случайное число в пределах от 0 до 1
  
  * randomGaus - случайное число в пределах от -1 до 1 с распределением по Гаусу
  
  ### Управление камерой
  
         {"Camera":{"x":"0","y":"0","z":"0","rotationY":"0","moveFactor":"0.5","rotFactor":"0.5","zoom":"1.0"}}
         
### Управление камерой
        {"Juniverse":{"tableHeight":"2"}}
        
         
      
