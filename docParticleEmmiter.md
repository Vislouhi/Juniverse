## ParticleEmmiter

### Излучатель частиц. Для моделлирования эффектов дыма, воды, и огня.

#### Cинтаксис

    [particleEmmiter1]
    
    
#### Коментарий

     [//particleEmmiter1]
   
#### Пример

    [particleEmmiter1]
    particleTexture=["fire1.png","fire2.png","fire3.png"]
    position={"x":"-0.1+0.2*random+mainX","y":"mainY","z":"-0.1+0.2*random+mainZ"}
    scale=0.5
    velocity={"x":"0","y":"0.01","z":"0"}


   
#### Скрипты
     //Выпустить частицу из particleEmmiter1 20 раз с шагом по времени 0.001с и временем жизни 0.8с
     {"ParticleEmmiter":{"item":1,"emmitNumber":20,"timeStep":0.001,"ttl":0.8}}





### Ключи

* particleTexture=["fire1.png","fire2.png","fire3.png"]

Набор текстур, которые будут воспроизводиться в случайном порядке

* position={"x":"-0.1+0.2*random+mainX","y":"mainY","z":"-0.1+0.2*random+mainZ"}

Позиция частицы может быть задана числом или формулой

* scale=0.5

Размер частицы

* velocity={"x":"0","y":"0.01","z":"0"}

Скорость частицы
