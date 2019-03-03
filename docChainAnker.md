## ChainAnker

### Крепление для объектов в пространстве к заданным координатам

#### Cинтаксис

    [chainAnker1]
    
    
#### Коментарий

     [//chainAnker1]
   
#### Пример

    [chainAnker1]
    childObjects=[2,5]
    hint={"fileName":"model/examles/hints/hang.png","x":20,"y":30,"w":20,"h":20}
    maxItems=10
    position={"x":"0","y":"-0.5+4*sin(ugol)","z":"-4*cos(ugol)"}
    shift={"x":"0","y":"0.3","z":"0"}
    step={"x":"0","y":"-0.5","z":"0"}
    radius=1.0
    writeNumberOfObjectsTo=mass1

#### Скрипты
        [script(example)]
        //Снять с chainAnker1 последний элемент
        {"ChainAnker":{"item":"1","action":"dropLast"}}
       


### Ключи

* childObjects=[2,5]

Номера объектов, которые могут быть закреплены

* hint={"fileName":"model/examles/hints/hang.png","x":20,"y":30,"w":20,"h":20}

Всплывающая подсказка

* maxItems=10

Количестово объектов, которое может быть закреплено

* onAddItem=addScript

Скрипт, который будет выполнен при закреплении объекта

* onDropItem=dropScript

Скрипт, который будет выполнен при снятии объекта

* position={"x":"0","y":"-0.5+4*sin(ugol)","z":"-4*cos(ugol)"}

Позиция объекта, может быть задана числом, или формулой

* shift={"x":"0","y":"0.3","z":"0"}

Первый объект будет закреплен с этим сдвигом относительно начала

* step={"x":"0","y":"-0.5","z":"0"}

Шаг, с которым будут подвешиваться объекты

* radius=1.0

Радиус примагничивания объектов

* writeNumberOfObjectsTo=mass1

Указатель на переменную, в которой хранится количество подвешанных объектов
