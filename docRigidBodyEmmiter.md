## RigidBodyEmmiter

### Излучатель твердых тел. 

#### Cинтаксис

    [rigidBodyEmmiter1]
    
    
#### Коментарий

     [//rigidBodyEmmiter1]
   
#### Пример

    [rigidBodyEmmiter1]
    emmitRigidBody=1


   
#### Скрипты
     //Выпустить твердое тело из rigidBodyEmmiter1 2 раза с шагом по времени 0.5с и временем жизни 3.5с
     {"EmmitRigidBody":{"item":"1","number":"2","timeStep":"0.5","ttl":"3.5"}}
     //Уничтожить все испущенные частицы эммитером rigidBodyEmmiter1
     {"EmmitRigidBody":{"item":"1","action":"clear"}}





### Ключи


* emmitRigidBody=1

Указывает какой объект RigidBody  следует испускать

* onEmmitFinished=reset

Указывает какой скрипт выполнить, когда испускание частиц закончится
