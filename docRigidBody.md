## RigidBody

### Модель твердого тела. Взаимодействует по законам физики с другими твердыми телами.

#### Cинтаксис

    [rigidBody1]
    
    
#### Коментарий

     [//rigidBody1]
   
#### Пример

    [rigidBody1]
    mode=sphere
    position={"x":"0.0","y":"3.6","z":"-0.3"}
    velocity={"x":"0.0","y":"0","z":"0.0"}
    mass=1.1
    gravity=10
    radius=0.05

   
#### Скрипты
     //Включить или выключить расчеты для rigidBody1
     {"RigidBody":{"item":"1", "state":"on"}}
     {"RigidBody":{"item":"1", "state":"off"}}
     //Поместить rigidBody1 в данное положение
     {"RigidBody":{"item":"1", "x":"1","y":"2","z":"3"}}
     //Задать rigidBody1 данную скорость
     {"RigidBody":{"item":"1", "velocityX":"0","velocityY":"0.1","velocityZ":"0"}}
     //Изменить длину пружинного соединения
     {"RigidBody":{"item":"1", "springConnection":{"index":1,"length":"0.3-0.1"}}}





### Ключи

* attenuation=10

Затухание движения твердого тела для сферического твердого тела

* attenuation={"tangent":"1","ortogonal":"0.3"}

Характеристкики затухания движения для твердого тела сложной формы.

tangent - затухание движения при качении по данному твердому телу

ortogonal - затухание движения при отскоке от данного твердого тела

* forceField={"x":"10-r*r","y":"-1","z":"0.0"}

Силовое поле, действующее на данное твердое тело, задается формулами

* gravity=10

Ускорение свободного падения, которое будет применяться к данному телу

* mode=mesh

Тип твердого тела, можеь быть "mesh" или "sphere"

mesh - твердое тело имеет форму, расчеты сталкновений будут ее учитывать

sphere - тело имеет сферическую форму

* mass=0.0

Масса тела

* mesh=plate.obj

Форма тела может быть загружена из файла

* position={"x":"0","y":"-0.5","z":"0.0"}

Начальная позиция твердого тела может быть задана только числом

* radius=0.1

Радиус сферы, только для сферических твердых тел

* rotation ={"x":"0.0","y":"1.0","z":"0.0","angle":"0"}

Поворот твердого тела, только для твердых тел, имеющих формулой

* springConnection1={"to":"2","length":"5.0","stiffness":"300","attenuation":300}

Пружинное соединение

to - объект rigidBody к которому подсоединен данный объект

length - длина пружины

stiffness - жесткость пружины

attenuation - затухание колебаний пружины

* useItemAsBody=1

Соответствующая модель item будет располагаться там же, где и твердое тело

* velocity={"x":"0.0","y":"0.0","z":"0.0"}

Начальная скорость движения твердого тела

* writePositionXTo=sharX

Указатель переменной, в которую будет заноситься x координата объекта

* writePositionYTo=sharY

Указатель переменной, в которую будет заноситься y координата объекта

* writePositionZTo=sharZ

Указатель переменной, в которую будет заноситься z координата объекта
