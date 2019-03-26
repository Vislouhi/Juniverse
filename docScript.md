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
    
#### Скрипты
       {"Script":{"execute":"script"}}
    

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
         
      
