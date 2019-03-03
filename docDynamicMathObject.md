## DynamicMathObject

### Решатель дифференциального уравнения второго порядка. Используется для моделирования движения по второму закону Ньютона.

#### Cинтаксис

    [dynamicMathObject1]
    
    
#### Коментарий

     [//dynamicMathObject1]
   
#### Пример

    [dynamicMathObject1]
    force=-5*ugol*reset-0.1*mass1*cos(ugol)+0.1*mass2*cos(ugol)
    attenuation=1
    value=ugol
    maxLimit=0.3
    minLimit=-0.3





### Ключи


* force=-5*ugol*reset-0.1*mass1*cos(ugol)+0.1*mass2*cos(ugol)

Сила действующая на тело, может быть задана чслом или формулой

* attenuation=1

Затухание движения

* value=ugol

Переменная, в которую будет записан результат вычислений

* maxLimit=0.3

* minLimit=-0.3

Значения, ограничивающие результат вычислений

* writeVelocityTo=vel

Перменная, в которую буде записываться скорость изменения результата вычислений.
