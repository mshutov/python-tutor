---
layout: page
permalink: /nachinaem-pisat/
---
# Начинаем писать

В качестве разминки предлагаю  написать простую функцию, которая при вызове будет запрашивать имя и после ввода имени выводить приветствие, например:

``` python-console
>>> hello_func()
Введите ваше имя: Михаил
Здравствуйте, Михаил!
```

Запросить информацию от пользователя поможет функция [input([текст])](https://docs.python.org/3/library/functions.html#input), вывод текста — с помощью [print()](https://docs.python.org/3/library/functions.html#print), которой можно передать любое количество строк.

Для первого задания будет решение, а далее — только подсказки.

Решение

``` python
def hello_func():
    name = input("Введите ваше имя: ")
    print("Здравствуйте, ", name, "!", sep='')
```

Далее — [приветствие в соответствии с временем суток]({{site.baseurl}}/privetstvie-v-sootvetstvii-s-vremenem-sutok/)