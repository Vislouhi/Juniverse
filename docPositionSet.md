## PositionSet

### Переключатель.

#### Cинтаксис

     [positionSet(positions)]
    
    
#### Коментарий

     [//positionSet(positions)]
   
#### Пример

      [positionSet(positions)]
      fileName=model/examles/meshes/positions.obj
      position={"x":"0","y":"5","z":"0"}
      scale=0.5

   
#### Скрипты
      //Распределить позиции positionSet(positions) между объектами item(s1), item(s2) , item(s3) , item(s4)  
      {"PositionSet":{"item":"positions","distribute":["s1","s2","s3","s4"]}}
      //Координаты позиции с индексом 2 записать в соответствующие переменные ["sX","sY","sZ"]
      {"PositionSet":{"item":"positions","index":"2","toVariables":["sX","sY","sZ"]}}





### Ключи

* fileName=model/examles/meshes/positions.obj

Имя файла из которого будут загружены позиции.

* position={"x":"0","y":"5","z":"0"}

Сдвиг всех позиций пространстве

* scale=0.5

Масштаб
